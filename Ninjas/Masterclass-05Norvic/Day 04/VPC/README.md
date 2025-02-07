# What's up in AWS VPC?

**AWS VPC (Virtual Private Cloud)allows one to launch AWS resources in a logically isolated virtual network.**

**What is VPC?**
-  launch a virtual network with the benefits of using the scalable infrastructure of AWS.

**Key Features**
-   Configuration of subnets, Ip addressing, routing, Gateways and endpoints
-   Peering connections - use it to route traffic between the resources in two VPC's.
-   Traffic Mirroring - Copy network traffic from interfaces and send it to monitoring for inspection.
-   VPC flow logs - Captures information about the traffic going to and from the VPC.

**How VPC Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowVPCWorks.png)

**Benefits**
-   Architecture - Customizable and the user has complete control of the network architecture.
-   Security - Enhanced and secure isolated environment.

**Use cases**
-   Hosting a public facing website, connecting to the internet via an internet gateway.

**Integration**
-   Both internet and Corporate Data Centre utilizing an internet Gateway and Virtual Private Gateway.

**Getting Started**
-   Setup VPC in the AWS Service Console and add resources like EC2, RDS instances.
-   Finally, configure VPCs to communicate with each other across availability zones.

**Best Practices**
-   Choose the appropriate VPC type and CIDR block, Isolate environment and use Multi-AZ deployments.

**Challenges and Solutions**
-   IP conflicts - Plan and design for scalability

**Pricing overview**
-   ![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/VPCPricing.png)

**Case Studies**
-   Host multi-tier web applications,create hybrid connections, launch a simple website.

**Conclusion**
-   AWS VPC is a core component that lets users create a virtual network which offers a secure and isolated environment.