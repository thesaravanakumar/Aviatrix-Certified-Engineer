## Feature Overview - Part 1 & Part 2

<img width="600" align="right" src="https://user-images.githubusercontent.com/59575502/203302560-46393574-6fdc-4a24-b1c4-804ca61f895d.png">

#### Agenda
- [Core Features](#CoreFeatures)
- [Transit](#Transit)
- [Ingress Security](#IngressSecurity)
- [Egress Security](#EgressSecurity)
- [High Performance Encryption](#HighPerformanceEncryption)
- [Site2Cloud](#Site2Cloud)
- [Routing Control](#RoutingControl)
- [SD-WAN Integaration](#SD-WANIntegaration)
- [User VPN](#UserVPN)
- [Firewall Inspection Best Practices](#FirewallInspectionBestPractices)
- [Aviatrix Integrated Stateful Firewall](#AviatrixIntegratedStatefulFirewall)
- [Transit FireNet](#TransitFireNet)
- [ThreatIQ with ThreatGuard](#ThreatIQwithThreatGuard)
- [Network Behavior Analytics](#NetworkBehaviorAnalytics)


<a name="CoreFeatures"></a>
### Core Features
It is not a SaaS or a managed service and it is yours (means it will be seen in your csp like vpc, vm's)

Components:
- **Controller**
  - Single controller for all the clouds.
  - Acts as a brain of the solution.
  - It is a multilingual entity meaning it can speak to native api's of the CSP's.
- **Gateways**
  - Represented by red circles arrows pointed towards each other.
  - You deploy gateways and their lifecycle directly from the controller either by UI or terraform provider.
- **3rd party API integaration**
  - You can achieve service insertion and chaining (meaning deploy next-gen firewall from aviatrix).
- **Copilot**
  - Represented by red icon that has a pilot hat.
  - Day 2 operations component platform which provide multi cloud operational visibility.
  - Gain visibility and control over your cloud network with Aviatrix CoPilot
   ```
      * Topology 
         - Interactive mapping and in-line troubleshooting for your cloud network
      * FlowlQ 
         - Detailed Network Analysis and Flow inspection
      * AppiQ 
         - End-to-End Application Path Inspection and Troubleshooting
      * ThreatiQ and ThreatGuard 
         - Multi-cloud native network security to identify and block traffic to known malicious destinations
      * Network Behavior Analytics
          - Uses your specific network characteristics to construct a behavioral baseline
          - Identifies and alerts on potential threats through abnormal network behavior
      * Micro-segmentation
          - Granular network security controls for distributed applications in the cloud
          - Dynamic, embedded solution that creates zero-trust enforcement with centralized policy management across multiple clouds
  ```

<a name="Transit"></a>
### Transit (core or backbone network)

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204084429-14aa248f-173e-4c8b-b759-8e30a0837abf.png">
<img width="1200" src="https://user-images.githubusercontent.com/59575502/204084432-e713dd7d-6d1e-4cce-8301-d08049e0069a.png">

<a name="IngressSecurity"></a>
### Ingress Security

<img width="400" align="right" src="https://user-images.githubusercontent.com/59575502/204084656-73082499-a49b-4d0d-88d8-76da6027fb38.png">

1. Orchestrate VPC Ingress Routing
2. Programmatically pull threat intelligence from GuardDuty
3. Programmatically create drop rules on Aviatrix Gateway based on Guard Duty Intelligence

<a name="EgressSecurity"></a>
### Egress Security

Egress FQDN Filtering can be applied in two manners.
  - centralised ```egress gateways are in transit layer.```
  - distributed ```egress gateways are in application (spoke) layer.```

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204085125-ef0fafad-a2fe-4e60-9449-10cfe4992587.png">

<a name="HighPerformanceEncryption"></a>
### High Performance Encryption

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204085261-5b078faf-14f7-4595-8ddd-95d57ced2875.png">

#### Solution: Aviatrix High-Performance Encryption (HPE)
- Aviatrix Controller automatically builds multiple tunnels between Aviatrix devices
- Uses all available CPU cores
- IPsec encryption performance can be up to 90 Gbps

<div align="center">
<img width="600" src="https://user-images.githubusercontent.com/59575502/204085360-e540086e-431c-430f-bec4-97f37fe93d1a.png">
</div>

## Feature Overview - Part 2

<a name="Site2Cloud"></a>
### Site2Cloud and other services that connect to external networks
<img width="600" align="right" src="https://user-images.githubusercontent.com/59575502/204087033-11f162cc-9353-40e8-91d4-6ca019745fbe.png">

- IPsec connection to Public Cloud:
  - On-Prem DC
  - 3rd Party Appliances, SD-WAN
  - Branch
  - Clouds Native Constructs (VPCs/VNets/VCNs)
- Easy to use and template-driven
- Built-in diagnostic tools
- Solves Overlapping IPs Challenges

<img width="900" src="https://user-images.githubusercontent.com/59575502/204087253-bd59974d-65a5-4dfe-8c6e-8c7f62eb8bb9.png">

<a name="RoutingControl"></a>
### Routing Control

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204087633-0e4cdd63-e778-493c-a908-cc68e772012c.png">

<a name="SD-WANIntegaration"></a>
### SD-WAN Integaration

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204087813-0956ce1b-5bd5-4254-8f31-3665e86d97e6.png">

<a name="UserVPN"></a>
### User VPN

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088062-965318fa-7800-462e-a8e9-6a146f83460e.png">

<a name="FirewallInspectionBestPractices"></a>
### Firewall Inspection Best Practices

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088147-ea89c0ef-7223-4e14-b0b9-f42396ec5978.png">


<a name="AviatrixIntegratedStatefulFirewall"></a>
### Aviatrix Integrated Stateful Firewall

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088252-30cc856a-860a-46c5-841b-a372d3c71ff0.png">


<a name="TransitFireNet"></a>
### Transit FireNet

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088481-f09730b5-86b3-48de-9f0b-e4370376919e.png">
<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088483-91b4a488-c80a-4824-8c49-e0b84ef3c406.png">
<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088486-c08682a1-2b8a-4ad0-927f-9f3f8288af45.png">

<a name="ThreatIQwithThreatGuard"></a>
### ThreatIQ with ThreatGuard

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088857-060ba542-ed15-414a-8ec0-0416d07fdadf.png">

<div align="center">
<img width="600" src="https://user-images.githubusercontent.com/59575502/204088852-a5f9bb90-2d93-44da-945c-9fe1d33f0957.png">
</div>

<a name="NetworkBehaviorAnalytics"></a>
### Network Behavior Analytics

<img width="1200" src="https://user-images.githubusercontent.com/59575502/204088957-c5930dc6-a18d-4bf8-8b1f-d8a2ec39476b.png">

<div align="center">
<img width="600" src="https://user-images.githubusercontent.com/59575502/204088965-5ad8cb2e-0edd-4c19-a3d7-80acb4bfa7ed.png">
</div>
