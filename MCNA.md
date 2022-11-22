## What is MCNA?

Multi-cloud is a model of cloud computing where an organization utilizes a combination of clouds—which can be two or more public clouds, two or more private clouds, or a combination of public, private and edge clouds—to distribute applications and services.

<img width="1200" src="https://user-images.githubusercontent.com/59575502/203290046-14a5652e-f555-4271-82df-19453ecf8718.png">

### Reference architecture:

- These are blue prints or building blocks that can be repeated which is the main benifits of reference architecture.
- ```Left side``` of the picture is cisco model from 1990 for building data center networks.
- ```right side``` of the picture is adopted from late 2000.
<img width="1200" src="https://user-images.githubusercontent.com/59575502/203290208-c737c725-acbb-44f1-a38b-0345fbcdb3fe.png">

### What is Transit:

- Transit is entity that enables **communications at spokes**, connects multiple cloud and on-premise.
- You can have a single transit or multiple transit in a region each is responsible for different environment.
> spokes where the application is deployed

<img width="1200" src="https://user-images.githubusercontent.com/59575502/203290900-e42544a4-5f6a-4e51-ad96-6f21f9f06f31.png">

### Aviatrix provide Cloud Network Reference Architecture.

- The architecture has 3 pillars 
  - Security, 
  - ```Cloud networking``` has 3 layers 
      - application layer ```workloads in VPC's,VNET's,VCN's```
      - transit core backbone layer ```VPC's,VNET's,VCN's are connected to each other```
      - access layer ```which has on-prem connectivity``` 
  - Operations.

![image](https://user-images.githubusercontent.com/59575502/203291939-33233bf2-bbfe-4826-863b-8df758497281.png)

### Multi Cloud Reference Architecture
- When you go to multi-cloud the architecture is **same and repeat** itself.
- The approach for building one cloud is repeated when building multi cloud.

<img width="1200" src="https://user-images.githubusercontent.com/59575502/203293570-226ad7a4-b96e-4e77-bce4-2888f4bd2648.png">

#### ```transit peering``` - connecting multiple cloud transits ( eg:- connecting aws transit to azure transit )

<img width="1200" src="https://user-images.githubusercontent.com/59575502/203296085-c3288a81-ff96-48ef-bae8-213a8aa9af2d.png">



### Features
<img width="1200" src="https://user-images.githubusercontent.com/59575502/203293884-cd4a5920-0530-4b1d-8f9f-917fa11372ed.png">























