# About Aviatrix
Aviatrix is a cloud native networking company. Unlike any other networking vendors, the Aviatrix software platform understands the cloud provider’s native constructs. This allows you to leverage and control the native constructs directly using the cloud provider’s APIs extending their capabilities and integrating them into our software to provide organizations with turn key solutions accelerating your cloud journey.

<div align="center">
<img width="1200" src="https://user-images.githubusercontent.com/59575502/201621216-e82adc00-607b-488a-be77-98dc16f72e78.png">
</div>

#### Some common enterprise use cases are shown below:
- ```Datacenter to cloud``` ([Aviatrix Transit Network solution](https://docs.aviatrix.com/HowTos/transitvpc_workflow.html))
- ```Scalable Firewall deployment in the cloud``` ([Firewall Network](https://docs.aviatrix.com/HowTos/firewall_network_faq.html))
- ```Cloud to cloud VPN``` (Encrypted [peering connectivity](https://docs.aviatrix.com/HowTos/peering.html) in a cloud and multi cloud )
- ```User to cloud VPN``` (Remote user VPN (OpenVPN® based [SSL](https://docs.aviatrix.com/HowTos/uservpn.html) VPN solution) for developers)
- ```Site to cloud VPN``` (Branch and customer [sites to cloud](https://docs.aviatrix.com/HowTos/site2cloud_faq.html))
- ```Multicloud VPN``` ([Multicloud Peering](https://docs.aviatrix.com/HowTos/GettingStartedAzureToAWSAndGCP.html))

#### The complexity of the cloud networking comes from the following areas and they only grow as time goes on:
<img width="600" align="right" src="https://user-images.githubusercontent.com/59575502/201535033-cb233a11-06db-4b1f-817f-568687dca024.png">

1. Unprecedented Scale
2. Security
3. Unprecedented Performance
4. Skills Gap
5. Interoperability

#### Features of Aviatrix
- Centralized Controller
- Operational Visibility
- Multiple Accounts and Clouds
- Security & Compliance
- Simplify with Automation
- Faster Troubleshooting
- Integrated Analytics

#### Changing Center of Gravity
- Apps moving to public cloud
- Network and security services follow apps
- Complexity increasing inside the cloud
- Data Center, Branches, Customers, Partners connect to Public Clouds

![image](https://user-images.githubusercontent.com/59575502/201621943-eb5ece69-5a42-4467-936d-9a255ea1b2b3.png)

### Public Cloud Basics
Public Cloud is just someone else's data center. Your data center is/was not perfect and had issues. Data Centers of Cloud Service Providers are no different.
Except you have no visibility or control over it

#### Region
- Data Centers are grouped in geographic regions to provide service availability
    - Azure: 60+, AWS: 26+, GCP: 24+, OCI: 30+ 

#### Availability Zone (Data Center)
- Distinct locations within a region that are engineered to be isolated from failures
- Inexpensive, low-latency network connectivity to other Availability Zones in the same region
- Not all CSPs have regions with multiple Availability Zones 
   - Fault Domains / Availability Domains offer multiple racks/power lines for redundancy 
- AZs are randomized outside of an account

<div align="center">
  
| **Function**                   | **Comments**                                                   |
|:------------------------------:|:--------------------------------------------------------------:|
| Identity and Access Management | Who can do What to Which resource                              |
| Service                        | Compute, Storage, Network, Database                            |
| Resource                       | Specific instances that you can create (aka Constructs)        |
| Virtual Data Center            | Collection of resources that you can create within a geography |
| Dedicated Connectivity         | Private path connectivity from on-prem to SP region            |

</div>

<img width="1295" alt="Screenshot 2023-02-07 at 10 50 04 PM" src="https://user-images.githubusercontent.com/59575502/217317363-dc96927e-3f8a-4a71-aea4-8bb2eb7d4e4b.png">
<img width="1295" alt="Screenshot 2023-02-07 at 10 50 18 PM" src="https://user-images.githubusercontent.com/59575502/217317432-18d85cc7-3ed2-4fbc-9566-cdf5391b4b0d.png">

















