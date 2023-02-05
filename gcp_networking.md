# GCP Networking 101
### Hierarchy

### VPC
- If you create a VPC the ```Internet Gateway``` (allows connectivity to internet) and ```VPC Routing``` (routes traffic between VM's) is automatically created.
- VPC is ```Global``` but subnets are ```regional```.

<div align="center">
<img width="1200" src="https://user-images.githubusercontent.com/59575502/216826328-92259f17-4dd9-400e-a0c3-1a55be060264.png">
</div> 

### VPC Network and Subnets
- VPC networks don't have a top-level CIDR associated with them (IP ranges are defined at the subnet level)
- VPC networks consist of one or more subnets
- VPC Subnets can be created in
  - Auto Mode (creates subnets in each region automatically)
  - Custom Mode (VPC networks start with no subnets) [best practice]
  - You can create more than one subnet per region

<img width="1200" align="left" src="https://user-images.githubusercontent.com/59575502/216826158-a1540ec6-738c-44ac-987d-1dc9418b6cae.png">
</br>

### GCP Global VPC Design Caveats/Limitations
- Not a good design choice for enterprises
- Massive Blast Radius
  - All the subnets, irrespective of the region are inherently routable within a VPC
- No policy-based segmentation within the VPC
  - Manually create L4 stateful firewall rules
- NGFW Service insertion is not possible
  - The next hop for a VPC subnet route cannot be modified
  - A more specific route cannot be created either
- Encryption within the VPC is the best effort
- A design built around GCP Global VPC is not a Multi-Cloud Design

### GCP VPC Design Best Practices
Create multiple region-bound VPCs to secure your network by means of
- Segmentation
- Encryption
- Service Insertion

### GCP Shared VPC
<img width="386" align="right" src="https://user-images.githubusercontent.com/59575502/216827027-f71346b6-4650-4d60-9a90-8fcf0e3e9ac4.png">

- Use case
  - Centralize the control of network resources like subnets, routes, and firewalls
  - Improve the security by restricting network resources control to only network teams
- A Shared VPC is a VPC defined in a host project
  - Governance level concept for providing networking services to tenant VPCs
  - Made available as a centrally shared network for eligible resources in service projects
- A Service Project is a project that has been attached to a host project
  - It is given VPC(s) or subnet(s) by a Shared VPC Admin
- All VPCs must be in the same organization
- Each service project can only be attached to a single host project
- Shared VPC is not a transit replacement
- Shared VPC has no Control Plane or Data Plane → IAM construct 
- "Shared VPC" is not equal to "Shared Services VPC"
  - Not necessarily meant to be hosting shared services in the shared VPC

### Cloud Interconnect
<img width="386" align="right" src="https://user-images.githubusercontent.com/59575502/216827422-4716cd28-7f1a-4e5b-abce-54e31dece035.png">

- Connect on-prem network to VPC network through a private circuit
- Two types of Cloud Interconnect
  - Dedicated Interconnect
    - Meet the GCP network in a colocation facility
    - 10 Gbps or 100 Gbps pipes
  - Partner Interconnect
    - Connect to service providers that connect directly to Google
    - 50 Mbps to 50 Gbps
    - Layer 2 or Layer 3 connections are supported
- Both support multiple VLAN attachments for redundancy
> Limited encryption support

###Compute Engine
#### Typical features
- Google Cloud Platform can run VM instances
- Instance sizes range from tiny Shared Core VMs to massive machines with hundreds of cores with terabytes of RAM
- VMs are deployed in Availability Zones within a Region
- Managed Instance Groups enable VMs to scale up or down based on an image
#### Caveats
- Compute Engine VMs are Zonal
- NICS cannot be added to or removed from a VM after deployment
- A VM cannot have more than one NIC in a VPC
- Max. NIC count per VM is 8

### 3rd Party Firewall Service Insertion
<img width="600" align="right" src="https://user-images.githubusercontent.com/59575502/216827784-051b90b9-6a31-4544-926c-f3215fae3f61.png">

- Limits with Global VPC - Firewall insertion effectively regionalizes VPCS
  - The default VPC subnet routes cannot be overridden, making workloads in the same VPC unable to be inspected
  - The 3rd party Firewall VM is regionalized in a Managed Instance Group
- 3rd party Firewall Insertion design requires a VM with multiple NICs in different VPCs
  - NIC count is limited by vCPU number or a maximum of 8
  - NICs cannot be added or removed after creating the VM
  - VPC Peering can be used to increase the number of VPCs inspected but has its own limits

### Google Kubernetes Engine (GKE)
- GKE provides a managed environment for deploying, managing, and scaling containerized applications
  - Specific components like etcd are managed and backed up by Google
  - Node lifecycle is managed by Google (autoscaling, updates, etc.)
    - Nodes are VMs in a Managed Instance Group
- GKE offers two networking modes for node to node and pod to pod communication
  - VPC Native Networking (default)
  - Route Based Networking
- VPC Native Networking mode
  - Nodes (VMs) use IPs from primary VPC CIDR range
  - Pod and Service use IPs from secondary CIDR range (Alias IP Range)

#### Load Balancing
GCP Load Balancers generally target VM instances, but other endpoints are supported
- HTTP(S) Load Balancers and Reverse Proxy Load Balancers
  - Unlike AWS/Azure, GCP Load Balancers are fabric-level services; no ALB or AppGW is deployed
  - The traffic source IP is changed to a Google Public IP
  - Available in Global/Regional and External/Internal designs
  - Supports limited ports - 80/8080/443
  - External HTTPS Load Balancers support Cloud Armor/CDN
- TCP/UDP (Layer 4) Load Balancers
  - Available in External/Internal designs; Regional only
  - Internal Load Balancers support "all-ports" for use with Firewalls and Routing Appliances
  - Operate in Direct Server Return mode - the destination IP at the VM instance is the same as the Load Balancer IP
- TCP/SSL Proxy Load Balancers
  - External and Global
  - Has a specific list of ports supported
  - Traffic source IP is changed to a Google Public IP

### Google Cloud VPN - High Available (HA) VPN
- Types
  - HA VPN (current) 
  - Classic VPN (old/deprecated)
- The HA VPN connects a VPC to an external network using IPsec and BGP
  • Datacenter (Palo Alto, Cisco, etc.)
  • HA VPN Gateways
  • Other Clouds (AWS, Azure, etc.) 
- HA VPN Gateway cannot connect to a Virtual Appliance (VM) running in GCP 
- The HA VPN Gateway is deployed as a pair with two Public IP Endpoints
- Multiple remote endpoints and tunnels can be configured, allowing a full mesh (crisscross) to a pair of data center devices

### Private Access to Google APIs, Services, and Serverless
- Requirement
  - Applications/Workloads/VPC/VMs have a requirement to connect to various Google APIs, Services and Serverless
  - Public access is available, but some enterprises mandate Private (RFC 1918) access
- You can connect VPC/VM to the following Google offering without using Public IP addresses:
  - Connect to Google APIs
  - Connect to Services
  - Connect to Google Serverless (GCP Functions, Cloud Run, and App Engine)

<div align="center">
<img width="1200" src="https://user-images.githubusercontent.com/59575502/216828712-bd47b075-d910-49e9-bac3-3620d192485f.png">
</div>  

### Design Choices: Private Access to Google APIs, Services and Serverless
- Private Access to Google APIs using
  - PSC and/or PGA can be used. They both support most Google APIs and Services
  - PSC is preferred → Supply an unused IP to the endpoint and configure DNS
  - A PSC for Google APIs can be accessed from on-premise or peered regions, assuming proper DNS configuration
  - PGA can be enabled at the subnet level for VMs without Public IPs
- Private Access to Services
  - PSC and PGA can be used. They both support most Google APIs and services
  - PSC is preferred
  - PSA can also be used but it supports only some Google APIs or services
- VPC Private Access to Google Serverless
  - "VPC Connector" is the only option here

### Network Connectivity Center (NCC)
- What is it?
  - A hub and spoke model where the hub is a Google construct consisting of at least one cloud router and spokes
  - Spokes can be Cloud Interconnect circuits, Cloud VPN connections, or third-party virtual instances (called Router Appliances)
- Limitations
- The same VPC network must connect all spokes to the hub
- No multi-cloud support

<div align="center">
<img width="516" src="https://user-images.githubusercontent.com/59575502/216828936-ddfac93a-5c1f-4723-a29d-d1a4cffcf6c1.png">
</div>
