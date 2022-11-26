## Feature Overview - Part 1

<img width="600" align="right" src="https://user-images.githubusercontent.com/59575502/203302560-46393574-6fdc-4a24-b1c4-804ca61f895d.png">

#### Agenda
- [Core Features](#CoreFeatures)
- [Transit](#Transit)
- [Ingress Security](#IngressSecurity)
- [Egress Security](#EgressSecurity)
- [High Performance Encryption](#HighPerformanceEncryption)


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
