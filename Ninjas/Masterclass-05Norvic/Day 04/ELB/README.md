[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# ELB (Elastic Load Balancer)

**What is ELB?**
-  A service to distribute traffic using multiple servers like EC2 instances for easier workload distribution.

**What is it for?**

-   It helps with easing the workload being done by servers to ensure there are no issues like latency or failure.

**Examples:**

-   Website hosting, video streaming, mobile applications

**Key Features**
-   High throughput - designed to handle traffic as it grows.
-   Availability - distribute traffic across a single or multiple availability zone.
-   Health Checks - Insight to the health of applications.
-   Security - Create managed security groups.

**How ELB Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowELBWorks.png)

**Benefits**
-   Automatic scaling, Security, and Monitoring in real time.

**Use cases**
-   Modernize application with serverless and containers, Improve hybrid cloud network scalability.

**Integration**
-   Integrate API Gateway wit a public Application Load Balancer

**Getting Started**
-   Setup either an Application Load Balancer, Network Load Balancer, or Gateway Load Balancer through CLI or Console.

**Best Practices**
-   Optimize client connections by using connection pooling which re-uses connections.

**Challenges and Solutions**
-   Lack of reliability - deploy services and distribute traffic in multiple availability zones.

**Pricing overview**
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/ELBPricing.png)

**Case Studies**
-   Retain existing network appliance, scale modern applications without complex configurations.

**Conclusion**
-   AWS ELB is a service that distribute network traffic to improve application scalability.

