## What is Cloud Computing?
**Cloud Computing** means storing and accessing the data and programs on remote servers that are hosted on the internet instead of the computer’s hard drive or local server. Cloud computing is also referred to as Internet-based computing, it is a technology where the resource is provided as a service through the Internet to the user. The data that is stored can be files, images, documents, or any other storable document.

The following are some of the Operations that can be performed with Cloud Computing

- Storage, backup, and recovery of data
- Delivery of software on demand
- Development of new applications and services
- Streaming videos and audio

### Architecture of Cloud Computing:
**Cloud computing** architecture refers to the components and sub-components required for cloud computing. 
These components typically refer to:

1. Front end ( Fat client, Thin client)
2. Back-end platforms ( Servers, Storage )
3. Cloud-based delivery and a network (Internet, Intranet, Intercloud)

<center>
<img src = "https://media.geeksforgeeks.org/wp-content/uploads/20240429101404/Cloud-Computing-Architecture.webp" width="300px">
</center>

### Cloud Computing Services:
The following are the types of cloud computing services:
1. Onsite &rarr; 
2. IAAS &rarr; Infrastructure as a service
3. PAAS &rarr; Platform as a serice
4. SAAS &rarr; Software as a Service
5. FAAS &rarr; Functional as a service
<center>
<p float="left">
  <img src="https://miro.medium.com/v2/resize:fit:1400/0*KwBUDmIzCPhUOnqn.jpg" width="300" style="margin-right: 20px;">
  <img src="https://www.koyeb.com/_next/image?url=%2Fstatic%2Fimages%2Fblog%2Ftable-responsibilities-faas-vs-caas.png&w=1920&q=75" height="220"width="300"> 
</p>
</center>

1. **Infrastructure as a Service (IaaS)**
    - Flexibility and Control: IaaS comes up with providing virtualized computing resources such as VMs, Storage, and networks facilitating users with control over the Operating system and applications.
    - Reducing Expenses of Hardware: IaaS provides business cost savings with the elimination of physical infrastructure investments making it cost-effective.
    - Scalability of Resources: The cloud provides in scaling of hardware resources up or down as per demand facilitating optimal performance with cost efficiency.
2. **Platform as a Service (PaaS)**
    - Simplifying the Development: Platform as a Service offers application development by keeping the underlying Infrastructure as an Abstraction. It helps the developers to completely focus on application logic ( Code ) and background operations are completely managed by the AWS platform.
    - Enhancing Efficiency and Productivity: PaaS lowers the Management of Infrastructure complexity, speeding up the Execution time and bringing the updates quickly to market by streamlining the development process.
    - Automation of Scaling: Management of resource scaling, guaranteeing the program’s workload efficiency is ensured by PaaS.
3. **Software as a service (SaaS)**
    - Collaboration And Accessibility: Software as a Service (SaaS) helps users to easily access applications without having the requirement of local installations. It is fully managed by the AWS Software working as a service over the internet encouraging effortless cooperation and ease of access.
    - Automation of Updates: SaaS providers manage the handling of software maintenance with automatic latest updates ensuring users gain experience with the latest features and security patches.
    - Cost Efficiency: SaaS acts as a cost-effective solution by reducing the overhead of IT support by eliminating the need for individual software licenses.
4. **Function as a Service (FaaS)**
    - Event-Driven Execution: FaaS helps in the maintenance of servers and infrastructure making users worry about it. FaaS facilitates the developers to run code as a response to the events.
    - Cost Efficiency: FaaS facilitates cost efficiency by coming up with the principle “Pay as per you Run” for the computing resources used.
    - Scalability and Agility: Serverless Architectures scale effortlessly in handing the workloads promoting agility in development and deployment.

### Cloud Deployment Models
1. **Public Cloud:** A Public Cloud is Cloud Computing in which the infrastructure and services are owned and operated by a third-party provider and made available to the public over the internet. The public can access and use shared resources, such as servers, storage, and applications and the main thing is you pay for what you used. . Examples of public cloud providers – are Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP)

2. **Private Cloud:** A Private Cloud is a cloud computing environment in which the infrastructure and services are owned and operated by a single organization, for example, a company or government, and it is accessed by only authorized users within that organization. Private Cloud organizations have their own data center. private cloud provides a higher level of security. Examples – HPE, Dell, VMware, etc.

3. **Hybrid Cloud:** A hybrid cloud is a combination of both public and private cloud environments that allows organizations to take advantage of the benefits of both types of clouds. It manages traffic levels during peak usage periods  It can provide greater flexibility, scalability, and cost-effectiveness than using a single cloud environment. Examples – IBM, DataCore Software, Rackspace, Threat Stack, Infinidat, etc.



## AWS Global Infrastructure

The AWS Global Infrastructure **gives you the flexibility of choosing how and where you want to run your workloads, and when you do you are using the same network, control plane, API's, and AWS services.** If you would like to run your applications globally you can choose from any of the AWS Regions and AZs. ([AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/))

- AWS is a cloud computing platform which is globally available.
- Global infrastructure is a region around the world in which AWS is based. Global infrastructure is a bunch of high-level IT services which is shown below:
- AWS is available in 33 regions, and 105 availability zones 19 and 660 cloudFront POP's, 13 regional edge caches.

**The following are the components that make up the AWS infrastructure:**

1. Availability Zones
2. Region
3. Edge locations
4. Regional Edge Caches
<center>
<img src="https://static.javatpoint.com/tutorial/aws/images/aws-global-infrastructure.png" width="450">
</center>
<br>

1. **Availability zone as a Data Center:**
- An availability zone is a facility that can be somewhere in a country or in a city. Inside this facility, i.e., Data Centre, we can have multiple servers, switches, load balancing, firewalls. The things which interact with the cloud sits inside the data centers.
- An availability zone can be a several data centers, but if they are close together, they are counted as 1 availability zone.
2. **Region:**
- A region is a geographical area. Each region consists of 2 more availability zones.
- A region is a collection of data centers which are completely isolated from other regions.
- A region consists of more than two availability zones connected to each other through links.
- Availability zones are connected through redundant and isolated metro fibers.

<center>
<img src = "https://static.javatpoint.com/tutorial/aws/images/aws-global-infrastructure2.png" width="200">
</center>

3. **Edge Locations:**
- Edge locations are the endpoints for AWS used for caching content.
- Edge locations consist of CloudFront, Amazon's Content Delivery Network (CDN).
- Edge locations are more than regions. Currently, there are over 150 edge locations.
- Edge location is not a region but a small location that AWS have. It is used for caching the content.
- Edge locations are mainly located in most of the major cities to distribute the content to end users with reduced latency.
- For example, some user accesses your website from Singapore; then this request would be redirected to the edge location closest to Singapore where cached data can be read.
4. **Regional Edge Cache:**
- AWS announced a new type of edge location in November 2016, known as a Regional Edge Cache.
Regional Edge cache lies between CloudFront Origin servers and the edge locations.
- A regional edge cache has a large cache than an individual edge location.
- Data is removed from the cache at the edge location while the data is retained at the Regional Edge Caches.
- When the user requests the data, then data is no longer available at the edge location. Therefore, the edge location retrieves the cached data from the Regional edge cache instead of the Origin servers that have high latency.