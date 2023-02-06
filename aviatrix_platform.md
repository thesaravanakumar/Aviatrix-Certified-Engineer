# Aviatrix Platform Overview

## Controller
### Controller Dashboard 
Contains (csp accounts onboarded, avx gateways, spoke tunnels, firenet, fqdn deployments, active vpn users and sitetocloud connections)
<img width="1297" alt="Screenshot 2023-02-06 at 5 40 39 PM" src="https://user-images.githubusercontent.com/59575502/216967964-eafc4431-866d-4683-b97e-22133d496e7f.png">

### Onboarding Menu
<img width="1297" alt="Screenshot 2023-02-06 at 5 42 58 PM" src="https://user-images.githubusercontent.com/59575502/216968357-c73d314c-0e3f-4f43-8670-c613a3b0ec1d.png">
<img width="1297" alt="Screenshot 2023-02-06 at 5 43 59 PM" src="https://user-images.githubusercontent.com/59575502/216968558-c0f7fde1-d3ed-4834-b04a-089f2515bda9.png">

### Accounts Menu
Manages csp accounts, subscriptions, projects, RBAC.
<img width="1297" alt="Screenshot 2023-02-06 at 5 44 18 PM" src="https://user-images.githubusercontent.com/59575502/216968623-4292deb5-0029-447c-b01f-ea527bbe76cc.png">

### Gateway Menu
Manages life-cycle of all your Gateways.
<img width="1297" alt="Screenshot 2023-02-06 at 5 45 37 PM" src="https://user-images.githubusercontent.com/59575502/216968872-d408a2b8-3814-40a2-9025-4b46d79386db.png">

## Multi-cloud Transit Menu
Manages transit and spoke gateways
<img width="1297" alt="Screenshot 2023-02-06 at 5 53 51 PM" src="https://user-images.githubusercontent.com/59575502/216970494-ae3b9b86-82de-427f-9fad-ee01a3d54de0.png">

<img width="1297" alt="Screenshot 2023-02-06 at 5 55 21 PM" src="https://user-images.githubusercontent.com/59575502/216970772-d85011f5-aca9-422d-8280-26617045ba7c.png">

#### Likewise for spoke Gateways
Deployed in vpc,vnets and vcns where your application workloads are present.
<img width="1297" alt="Screenshot 2023-02-06 at 5 56 00 PM" src="https://user-images.githubusercontent.com/59575502/216970900-c5f30278-ba8b-4d96-997b-34c35845327d.png">
<img width="1297" alt="Screenshot 2023-02-06 at 5 56 31 PM" src="https://user-images.githubusercontent.com/59575502/216970997-fa879e9d-fd75-490e-9224-8f9305171da1.png">

#### Transit-Spoke attatchments which will create IPsec tunnels
<img width="1297" alt="Screenshot 2023-02-06 at 5 58 20 PM" src="https://user-images.githubusercontent.com/59575502/216971404-198760d1-0fcc-482d-8943-86e037b13f5d.png">

#### Create connection to external entity such as sitetocloud connection
Using Ipsec connections, GRE, LAN
<img width="1297" alt="Screenshot 2023-02-06 at 5 59 46 PM" src="https://user-images.githubusercontent.com/59575502/216971722-dcaf1a45-9d5a-472e-b865-bba1058b63bf.png">

### Multi-Cloud Transit List 
View your existing transit and spoke gateways
<img width="1297" alt="Screenshot 2023-02-06 at 5 59 46 PM" src="https://user-images.githubusercontent.com/59575502/216973648-a36743e2-9b1d-412d-a14c-63f26d9a705f.png">

### Transit Peering
Create and manage transit peerings (other csp or gateways in other regions)
<img width="1297" alt="Screenshot 2023-02-06 at 6 10 25 PM" src="https://user-images.githubusercontent.com/59575502/216973874-0efb9af8-7159-4012-8def-a58f229f2b5e.png">

### Firewall Network setup
setup firenet
<img width="1297" alt="Screenshot 2023-02-06 at 6 16 11 PM" src="https://user-images.githubusercontent.com/59575502/216975039-78b2f041-cbd1-46c4-aae7-a7341dc06eaf.png">

### Firewall Network List
View your existing firenet and firewall
<img width="1297" alt="Screenshot 2023-02-06 at 6 19 09 PM" src="https://user-images.githubusercontent.com/59575502/216975490-e75d37a2-7c42-46bf-8a16-390fb1191de5.png">

### Firewall Network Policy
To control which traffic should be service chained and redirected to firewalls
<img width="1297" alt="Screenshot 2023-02-06 at 6 19 09 PM" src="https://user-images.githubusercontent.com/59575502/216975561-675a4053-1d3d-4b43-bc33-68ddf670e311.png">

### CloudN
Setup and manage the lifecycle of aviatrix secure edge gateways.
<img width="1297" alt="Screenshot 2023-02-06 at 6 21 15 PM" src="https://user-images.githubusercontent.com/59575502/216975994-d5917a37-c5d7-4895-a0bd-3c7de64aefc5.png">

### SitetoCloud connections
Manage the lifecycle of sitetocloud connections
<img width="1297" alt="Screenshot 2023-02-06 at 6 26 02 PM" src="https://user-images.githubusercontent.com/59575502/216976931-67b834ce-d460-4c76-ba27-e475178b662d.png">

### OpenVPN Menu
Manages VPN access
<img width="1297" alt="Screenshot 2023-02-06 at 6 41 59 PM" src="https://user-images.githubusercontent.com/59575502/216980137-758b6056-da26-417f-b4cc-e8f457c80203.png">

### Security Menu
<img width="1297" alt="Screenshot 2023-02-06 at 6 43 41 PM" src="https://user-images.githubusercontent.com/59575502/216980472-d946a63e-b0e2-4676-bf22-50ed8db62d33.png">

#### Egress control sub menu
Configure Egress FQDN filtering.
<img width="1297" alt="Screenshot 2023-02-06 at 6 45 22 PM" src="https://user-images.githubusercontent.com/59575502/216980772-108cf6b9-5305-4379-b2c9-3e7095fc2d76.png">

## Copilot
### Copilot Dashboard
- It contains inventry of aviatrix gateways and shows where your cloud network deployed globally.
- Also there is a status check for each tile.
<img width="1297" alt="Screenshot 2023-02-06 at 6 46 28 PM" src="https://user-images.githubusercontent.com/59575502/216981045-71a66489-4e91-4203-90b6-70e2df35f44f.png">
<img width="1297" alt="Screenshot 2023-02-06 at 6 48 28 PM" src="https://user-images.githubusercontent.com/59575502/216981494-9d99e8da-d443-425a-88a6-c0d46bee7175.png">

### Traffic Dashboard
For the passed 24 hours you can see the traffic by region, (vpc,vnets,vcns), gateways and instances.
<img width="1297" alt="Screenshot 2023-02-06 at 6 49 26 PM" src="https://user-images.githubusercontent.com/59575502/216981682-0b3ff542-a6aa-4d30-9efd-d3bd990a628e.png">

### Topology
- Gives the global-topologycal view.
- Edit/Filter/Save the layout.
- Click on gateway to get content based diagnostics (ping, traceroute, tracepath, packetcapture.
<img width="1297" alt="Screenshot 2023-02-06 at 6 51 09 PM" src="https://user-images.githubusercontent.com/59575502/216982102-d68dbd4c-367b-405e-b966-0b27e34c59f7.png">

### FlowIQ
- Allows visualization of flow records that are generated by aviatrix gateways.
- Overview summarizes the top talkers.
<img width="1297" alt="Screenshot 2023-02-06 at 6 54 30 PM" src="https://user-images.githubusercontent.com/59575502/216982795-5232e607-1afa-4bd3-bc7f-261cca092816.png">

- Trends gives the movement of traffic at any time window you want.
<img width="1297" alt="Screenshot 2023-02-06 at 6 57 01 PM" src="https://user-images.githubusercontent.com/59575502/216983351-375457cc-2231-4651-a44f-312365ef1f5f.png">

- Geolocation shows you a heatmap view where traffic is going or comming from.
<img width="1297" alt="Screenshot 2023-02-06 at 6 57 25 PM" src="https://user-images.githubusercontent.com/59575502/216983437-9a7ddac0-a8f4-4335-9d02-df364991a2ce.png">

- Flows shows you the relationship between top talkers and top recievers. (left - source, right - destination) (thick line - most traffic)
<img width="1297" alt="Screenshot 2023-02-06 at 6 59 23 PM" src="https://user-images.githubusercontent.com/59575502/216983831-99e760ae-2495-4e40-ad42-b559beaf7e7e.png">

- Records gives you rows and column of datas.
<img width="1297" alt="Screenshot 2023-02-06 at 7 15 15 PM" src="https://user-images.githubusercontent.com/59575502/216987348-e797995f-3758-48c0-86e9-236737648062.png">

### Performance Menu
Gives you time series data over 50 metrics this include system metrics (memory and cpu) and network metrics that a csp exposes.
<img width="1297" alt="Screenshot 2023-02-06 at 7 16 32 PM" src="https://user-images.githubusercontent.com/59575502/216987637-054768fb-9928-41da-b1e3-b79636e1703f.png">

- create policies to scale your gateways based on certain threshold
<img width="1297" alt="Screenshot 2023-02-06 at 7 19 25 PM" src="https://user-images.githubusercontent.com/59575502/216988308-cf2cb632-82a8-4fe4-ad70-eab1d28ade73.png">

### Cloud Routes Menu
can locate routing tables and routes on gateways and (vpc, vnet)
- Gateway Routes
<img width="1297" alt="Screenshot 2023-02-06 at 7 20 04 PM" src="https://user-images.githubusercontent.com/59575502/216988478-5abf7f4e-758e-410a-ac85-5ab0aa524901.png">

- VPC/VNET Routes
<img width="1297" alt="Screenshot 2023-02-06 at 7 22 32 PM" src="https://user-images.githubusercontent.com/59575502/216989131-2c3b070e-99c3-4470-a99d-11678d1e5140.png">

- SitetoCloud connections
<img width="1297" alt="Screenshot 2023-02-06 at 7 23 30 PM" src="https://user-images.githubusercontent.com/59575502/216989378-5b9de7c0-3eb7-49e6-8eee-719d9d9c4cdc.png">

- BGP Info </br>
Gives you visual representation, learned and advertised CIDR routes
<img width="1297" alt="Screenshot 2023-02-06 at 7 25 07 PM" src="https://user-images.githubusercontent.com/59575502/216989768-71dfe18a-1acf-4851-8a1e-94225b2461a1.png">

### APPIQ </br>
Gives you a report of end to end path troubleshooting 
<img width="1297" alt="Screenshot 2023-02-06 at 7 27 17 PM" src="https://user-images.githubusercontent.com/59575502/216990273-452e8cdd-530a-4859-822c-91562abd6825.png">

### Security 
- Network Segmentation </br>
has network domain, logical view, physical view, regional view
<img width="1297" alt="Screenshot 2023-02-06 at 7 27 56 PM" src="https://user-images.githubusercontent.com/59575502/216990443-ba387cd3-d214-460b-a94b-1d6ac23b31cd.png">

- Micro-segmentation </br>
manages lifecycle of app domains and create policies to allow/decline traffic to app domains.
<img width="1297" alt="Screenshot 2023-02-06 at 7 33 41 PM" src="https://user-images.githubusercontent.com/59575502/216991711-22139f63-7e73-4533-94e6-f7191327790a.png">

### ThreadIQ
- Threads </br>
shows all the malicious IP's reported in the env (where why how) the thread occurs
<img width="1297" alt="Screenshot 2023-02-06 at 7 34 00 PM" src="https://user-images.githubusercontent.com/59575502/216991776-f1d10140-fd60-49b8-8f74-cc50e036bccd.png">

- Threadguard </br>
It programs stateful firewall rules and block the IP in both directions on all gateways.
<img width="1297" alt="Screenshot 2023-02-06 at 7 36 09 PM" src="https://user-images.githubusercontent.com/59575502/216992278-a4dbce32-a4a0-4050-9c9f-6339cdfd57bb.png">

### Anomalies Menu
Network behaviour analytics can be retrived
<img width="1297" alt="Screenshot 2023-02-06 at 7 37 33 PM" src="https://user-images.githubusercontent.com/59575502/216992594-920ad6e0-9854-4e1c-9795-d6b728d9dd3d.png">
