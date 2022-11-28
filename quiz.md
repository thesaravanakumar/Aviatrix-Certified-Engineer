## About Aviatrix

1. Where is the "center of gravity" in the new computing model?
    * [x] Public Cloud
    * [ ] Private Cloud
    * [ ] On-premises
    * [ ] Provider

2. What caused a large push to the public cloud?
    * [ ] IT Security pushed it
    * [x] Speed of Deployment
    * [ ] Lack of on-premises knowledge
    * [ ] Compliance reasons

3. As applications move to the cloud, their proximity to the Internet is:
    * [x] closer
    * [ ] farther away
    * [ ] exactly the same

4. What are common challenges that enterprises face in the cloud?
    * [ ] Lack of reference architecture
    * [ ] Lack of visibility and troubleshooting
    * [ ] Multi-Cloud support
    * [x] All of the above

5. How does Aviatrix help customers in public clouds?
    * [ ] Provides building blocks for AWS networking
    * [ ] Aviatrix is a visibility tool inside cloud networks
    * [x] Aviatrix is a multi-cloud platform that brings a consistent architecture with Day 2 Operations and Visibility
    * [ ] Aviatrix is an on-premises solution for networking and security

6. Which group led the initial charge in the cloud?
    * [x] DevOps
    * [ ] IT
    * [ ] Security
    * [ ] System Admistrators

7. True or false: When things break, DevOps teams can troubleshoot their own network connectivity without needing networking teams for support.
    * [ ] True
    * [x] False

8. Which unique challenge does a network engineer face in the cloud that is not present on-premises?
    * [ ] Routing
    * [ ] Firewalling
    * [x] Accounts/Subscriptions
    * [ ] Security

9. When organizations build in the cloud, the providers typically follow what model:
    * [x] Build it yourself - we provide the pieces
    * [ ] Plenty of reference architectures to choose from
    * [ ] Providers will design an architecture for you
    * [ ] None of the above

10. True or false: Cloud providers can easily help customers in multi-cloud deployments.
    * [ ] True
    * [x] False

## Introduction to Public Cloud Networking

1. What is the definition of a PaaS Service?
    * [ ] You as the customer own the entire stack
    * [x] You as the customer manage just the application and data
    * [ ] You as the customer just consume the service
    * [ ] None of the above

2. What is a hybrid cloud?
    * [ ] Multi-tenant cloud service provided by Microsoft, Amazon, etc.
    * [ ] Single-tenant cloud service hosted by you the customer
    * [x] A combination of Public and Private Cloud
    * [ ] Any virtualized compute provider

3. Which is NOT a valid component of the cloud?
    * [ ] Datacenter
    * [ ] Region
    * [x] Geographical Zone
    * [ ] Availability Zone

4. Is Availability Zone 1A the same for every customer in cloud environments?
    * [ ] Yes
    * [x] No

5. True or false: We have an architectural gap in the cloud today because there is no consistent framework for network and security across clouds.
    * [x] True
    * [ ] False

6. The On-Premises world is most similar to which type of service:
    * [ ] SaaS
    * [x] IaaS
    * [ ] PaaS
    * [ ] CSP

7. Office365 is an example of which service:
    * [ ] IaaS
    * [ ] PaaS
    * [x] SaaS
    * [ ] None of the above

8. True or false: A region is the same thing as a data center for cloud providers.
    * [ ] True
    * [x] False

9. True or false: When a cloud provider deploys a region, there are always multiple availability zones present.
    * [ ] True
    * [x] False

10. One advantage of availability zones includes:
    * [ ] Resources across AZs can survive a regional outage
    * [ ] Resources across AZs can survive a global outage
    * [x] Resources across AZs can survive a data center outage
    * [ ] None of the above

## AWS Networking 101

1. Which AWS service represents a virtual machine?
    * [ ] VPC
    * [ ] Direct Connect
    * [x] EC2
    * [ ] S3

2. True or false: To connect a VPC, AWS uses an implicit router that customers must configure to allow communication between VPCs.
    * [ ] True
    * [x] False

3. Which AWS service best represents your private virtual walled garden in the cloud?
    * [ ] Direct Connect
    * [x] VPC
    * [ ] IAM
    * [ ] CloudFront

4. True or false: In AWS, subnets are global resources spread across availability zones.
    * [ ] True
    * [x] False

5. Which AWS security component is a stateless filter?
    * [ ] Security Group
    * [x] NACL
    * [ ] Internet Gateway
    * [ ] Network Security Groups (NSG)

6. True or false: Security Groups in AWS cannot be shared across VPCs unless they are peered together.
    * [x] True
    * [ ] False

7. Which gateway is not an available option with AWS?
    * [ ] Internet Gateway
    * [ ] NAT Gateway
    * [x] Virtual Network Gateway
    * [ ] Transit Gateway

8. True or false: Transit Gateway in AWS fully automates routing so that no manual configuration is required.
    * [ ] True
    * [x] False

9. In AWS, a Direct Connect circuit can terminate on which of the following:
    * [x] Direct Connect Gateway
    * [ ] Transit Gateway
    * [ ] Internet Gateway
    * [ ] VPC Gateway

10. Using native AWS constructs, the highest available bandwidth within an IPsec tunnel is:
    * [ ] 500Mbps
    * [x] 1.25Gbps
    * [ ] 4Gbps
    * [ ] 10Gbps

11. True or false: There are currently no limitations to the number of routes supported in AWS Transit Gateway.
    * [ ] True
    * [x] False

## Azure Networking 101

1. What is the private circuit term in Azure that is analogous to Direct Connect in AWS?
    * [ ] Dedicated Interconnect
    * [ ] Partner Interconnect
    * [x] ExpressRoute
    * [ ] Fast Connect

2. What are Virtual Network Gateways used for?
    * [x] Hybrid Connectivity termination constructs for VPN or ExpressRoute
    * [ ] Native construct used for VNet peering
    * [ ] Native construct used for Internet access
    * [ ] Hybrid Connectivity option for SD-WAN connectivity

3. Which Azure component groups items together for better organizational control of a specific workload?
    * [ ] Service
    * [ ] Resource
    * [x] Resource Group
    * [ ] AD Tenant

4. What is the top-level organizational structure in Azure?
    * [ ] Resource Group
    * [ ] Subscription
    * [x] AD Tenant
    * [ ] Resource

5. True or false: In Azure, subnets are created as either private or public.
    * [ ] True
    * [x] False

6. Some challenges with Azure Virtual WAN as a platform include:
    * [ ] Limited visibility and troubleshooting
    * [ ] Does not provide a multi-cloud architecture
    * [ ] Limited third-party devices supported in the HUB
    * [x] All of the above

7. An ExpressRoute circuit in Azure can terminate on which device (select all that apply)
    * [x] ExpressRoute Gateway
    * [ ] NVA
    * [x] Virtual Network Gateway
    * [ ] VPN Gateway

8. True or false: Using ExpressRoute hairpinning for spoke-to-spoke traffic is the recommended option for transit within Azure.
    * [ ] True
    * [x] False

9. What is an NVA in Azure (Select all that apply)
    * [x] Any third-party device in the Azure marketplace
    * [ ] Any native Azure networking device
    * [ ] Network Virtual Access
    * [x] Network Virtual Appliance

10. Challenges with using an NVA to provide spoke-to-spoke communication in Azure include: (select all that apply)
    * [x] User-Defined Route Management at scale
    * [ ] No allocated bandwidth on edge routers
    * [ ] This method is a 1-to-1 mapping of VNets

## GCP Networking 101

1. A GCP private circuit is referred to as:
    * [ ] ExpressRoute
    * [ ] Direct Connect
    * [x] Cloud Interconnect
    * [ ] Fast Connect

2. True or false: All resources within GCP are either Global or Regional or both.
    * [ ] True
    * [x] False

3. A VPC is an example of a:
    * [ ] Zonal Resource
    * [ ] Regional Resource
    * [x] Global Resource
    * [ ] None of the above

4. For a single user, GCP resources are structurally organized in a:
    * [ ] Organization
    * [ ] Folder
    * [x] Project
    * [ ] Resource Group

5. True or false: GCP encourages deployments of multiple VPCs to spread out all your workloads.
    * [ ] True
    * [x] False

6. What does Auto Mode in GCP mean?
    * [ ] VPC networks start with no subnets
    * [x] subnets are created in each region
    * [ ] you must manually configure your subnets
    * [ ] address space will be defined at the VPC level

7. True or false: GCP supports dynamic routes within the cloud.
    * [x] True
    * [ ] False

8. True or false: VPC peering in GCP allows VPC to be transitive.
    * [ ] True
    * [x] False

9. A project can access another project's resource via (select all that apply)
    * [x] Shared VPC
    * [ ] Cloud Interconnect
    * [x] VPC Peering
    * [ ] Cloud Router

10. What are the caveats of a Global VPC design in GCP?
    * [ ] Massive blast radius
    * [ ] No policy segmentation within the VPC
    * [ ] Encryption within the VPC is best effort as per Google
    * [x] All of the above

## OCI Networking 101

1. What are virtual cloud networks called in OCI?
    * [ ] VPC
    * [x] VCN
    * [ ] OCI-NET
    * [ ] ORANET

2. True or false: OCI subnets can be tied to one or all Availability Domains in the region.
    * [x] True
    * [ ] False

3. True or false: DRG supports exactly 2 types of attachments: VCN and FastConnect.
    * [ ] True
    * [x] False (VCN, RPC, FastConnect, IPsec)

4. In OCI you need to specify a _____________ when creating resources.
    * [x] Compartment ID
    * [ ] Account Name
    * [ ] Oracle Prefix Identifier
    * [ ] Last 3 characters of tenancy id + the first three letters of your username

5. Service Gateways provide _____________ access from VCNs to Oracle Services.
    * [ ] Public
    * [ ] Hybrid
    * [x] Private
    * [ ] Round-robin hashed

6. Tenancy IAM metadata is bound to ___________________.
    * [ ] Company address
    * [x] Home region
    * [ ] Phoenix for all US customers
    * [ ] Globally, no restrictions

7. What are the two options for interconnecting VCNs within a region?
    * [x] Local Peering Gateway and DRG Attachments
    * [ ] There is none. It is a managed service, just like in AWS, Azure, and GCP.
    * [ ] Private Peering Gateway and DRG Attachments
    * [ ] Oracle Peering Gateway and Private Peering Connection

8. What does a Dynamic Routing Gateway in OCI do?
    * [ ] Terminate an IPsec tunnel from on-premises to OCI
    * [ ] Terminate a Fast Connect private circuit from on-premises to OCI
    * [ ] Achieve VCN peering between regions
    * [x] All of the above

9. True or false: DRGs within one OCI Region can be peered using an RPC.
    * [x] True
    * [ ] False

10. What is the benefit of Dynamic Routing Gateway attachments?
    * [ ] They support encryption by default
    * [x] They have their own route tables, which allow for flexibility
    * [ ] They are supported natively across all CSPs
    * [ ] They support overlapping IPs

## What is MCNA?

1. What are the three columns of the MCNA?
    * [ ] Management, Application, Cloud Networking
    * [x] Security, Cloud Networking, Operations
    * [ ] Management, Application, Operations
    * [ ] Authentication, Authorization, Management

2. What are the three layers of the MCNA?
    * [ ] Operations, Connectivity, and Core
    * [ ] Transit Core Backbone, Networking, and Applications
    * [ ] Access, Transit, and Management
    * [x] Application, Transit Core Backbone, and Access

3. True or false: Security and Visibility are inserted throughout the MCNA Architecture.
    * [x] True
    * [ ] False

4. Which answer is a benefit of having a Multi-Cloud Network Architecture?
    * [ ] Normalized Data Plane
    * [ ] Centralized Control Plane
    * [ ] Repeatable across cloud providers
    * [x] All of the above

5. What is the most important aspect of any multi-cloud network?
    * [ ] Access
    * [ ] Compute
    * [x] Transit
    * [ ] Delivery

6. The function of the cloud operations layer includes (select all that apply)
    * [ ] Multi-Cloud Centralized Visibility
    * [ ] Multi-Cloud Centralized Control
    * [ ] Multi-Cloud Centralized Orchestration
    * [x] All of the above

7. True or false: MCNA enables service chaining (i.e., insertion of firewalls).
    * [x] True
    * [ ] False

8. Cloud Access in MCNA provides common access for:
    * [ ] SDWAN
    * [ ] Direct Connect options from cloud providers
    * [ ] VPN connectivity
    * [x] All of the above

9. The core principle of MCNA is:
    * [ ] a cloud architecture per cloud using native constructs
    * [ ] an on-premises hybrid connectivity model for connecting to cloud
    * [ ] a security and visibility framework for cloud environments
    * [x] a multi-cloud network and security framework for consistent deployment across clouds

10. True or False: MCNA can only be applied to a multi-cloud environment.
    * [ ] True
    * [x] False

## Feature Overview - Part 1

1. An enterprise has workloads in AWS, Azure, and GCP. How many Aviatrix Controllers do they need?
    * [ ] 0
    * [x] 1
    * [ ] 2
    * [ ] 3

2. What is needed for workloads in two Segments to communicate with each other?
    * [ ] Deploy a third-party solution
    * [ ] Nothing. Segments are just labelling constructs.
    * [x] Configure a Connection Policy
    * [ ] Create a NACL

3. True or false: Aviatrix CoPilot can be used to write Terraform scripts.
    * [ ] True
    * [x] False

4. What is a challenge with native encryption within the cloud?
    * [ ] Cloud environments are not natively encrypted
    * [ ] Native encryption mechanisms are limited to 1.25G
    * [ ] IPsec tunnels are tied to a single core within compute
    * [x] All of the above

5. What are the components within the Aviatrix Platform?
    * [ ] Controller
    * [ ] Gateways
    * [ ] CoPilot
    * [x] All of the above

6. Why is cloud IPsec limited to 1.25G?
    * [x] Native solutions build tunnels across a single core only
    * [ ] This is can be overcome with multi-core VMs
    * [ ] Private connectivity like ExpressRoute and Direct Connect is encrypted by default
    * [ ] Cloud providers cannot provide encryption at all

7. True or false: The Aviatrix FQDN Egress Filter supports both centralized and distributed egress methods.
    * [x] True
    * [ ] False

8. True or false: Aviatrix can extend native AWS features like GuardDuty to provide enforcement of alerts.
    * [x] True
    * [ ] False

9. The advantage of Aviatrix Transit within the cloud is:
    * [ ] End-to-End Encryption
    * [ ] Repeatable across Clouds
    * [ ] Complete Visibility and Control
    * [x] All of the above

10. What does Multi-Cloud Network Segmentation provide?
    * [ ] Segmentation that can extend to on-premises
    * [ ] Segmentation of workloads that can meet auditing and compliance requirements
    * [ ] Segmentation across accounts, subscriptions, and projects
    * [x] All of the above

## Feature Overview - Part 2

1. What are some challenges with inserting firewalls in the cloud?
    * [ ] Repackaged Firewall Solution from on-premises world
    * [ ] Native Firewall Solutions are primarily L4 firewalls
    * [ ] Customer required to configure and manage routing
    * [x] All of the above

2. What is the advantage of the Centralized Stateful Firewall on Aviatrix Single AZ HA?
    * [ ] Separation of duties (App team manages instance security; Network team manages transit security)
    * [ ] No need for a load balancer
    * [ ] Multi-cloud repeatability
    * [x] All of the above

3. What advantages does the Aviatrix Site2Cloud offer?
    * [ ] Support for Network Address Translation (NAT)
    * [ ] Support for TCP and UDP tunnels
    * [ ] Uses a template-driven manner for configuration
    * [x] All of the above

4. True or false: Aviatrix FireNet can orchestrate the firewall deployment, firewall routing, and VNet/VPC routing for NGFW insertion.
    * [x] True
    * [ ] False

5. True or false: The Aviatrix User VPN solution does not allow profile-based granular access control.
    * [ ] True
    * [x] False

6. Which third-party integrations are available for Aviatrix User VPN?
    * [ ] DUO
    * [ ] Okta
    * [ ] AD
    * [ ] SAML
    * [x] All of the above

7. True or false: With Aviatrix Transit FireNet, workloads cannot be placed in different segments AND be inspected by NGFWs without losing visibility.
    * [ ] True
    * [x] False

8. True or false: Aviatrix can provide filtering of partner route advertisements through a BGP Approval Process.
    * [x] True
    * [ ] False

9. Which Aviatrix feature allows customers to group VPC/VNets with common security properties for access?
    * [ ] FireNet
    * [x] Security Domains (also known as Segments)
    * [ ] Site2Cloud
    * [ ] CloudWAN

10. True or false: Aviatrix Site2Cloud can also be used to onboard IoT devices.
    * [x] True
    * [ ] False

## Day 2 Operations

1. True or false: Aviatrix is a multi-cloud Terraform provider.
    * [x] True
    * [ ] False

2. True or false: Aviatrix cannot provide packet captures of live traffic.
    * [ ] True
    * [x] False

3. True or false: The VPC tracker is only available for AWS.
    * [ ] True
    * [x] False

4. What does Aviatrix use for Controller HA in AWS?
    * [ ] a Lambda script
    * [ ] an S3 bucket
    * [ ] an auto scaling group
    * [x] All of the above

5. How does FlightPath help users troubleshoot connectivity problems?
    * [ ] Allows the gateways to be access via API to perform queries
    * [ ] Provides a packet capture of specific network flows
    * [x] Provides a visual walk-through based on source and destination to highlight path issues
    * [ ] Provides ping and traceroute capabilities for source and destination

6. What are some operational challenges that customers face in the cloud?
    * [ ] Tier-3 becomes Tier-1 for troubleshooting
    * [ ] Limited visibility into native constructs
    * [ ] Lack of standard troubleshooting tools (ping, traceroute, etc.)
    * [x] All of the above

7. True or false: The Aviatrix Controller can perform auditing of routing constructs. This ensures that no new routes have been added that can affect end-to-end network correctness.
    * [x] True
    * [ ] False

8. True or false: Common troubleshooting tasks like ping and traceroute can be run from any Aviatrix gateway.
    * [x] True
    * [ ] False

9. What happens when the Aviatrix components require upgrades?
    * [ ] Downtime is required for all upgrades
    * [x] Upgrades are hitless
    * [ ] The controller must be rebooted after upgrades
    * [ ] The gateways must be rebooted after upgrades

10. Which of the following statements is true?
    * [ ] Customers must spin up a controller per subscription/account
    * [ ] Customers must spin up a controller per cloud environment
    * [ ] Customers can spin up a single controller but can only on-board one master account per cloud
    * [x] Customers can spin up a single controller and on-board multiple cloud accounts for management
