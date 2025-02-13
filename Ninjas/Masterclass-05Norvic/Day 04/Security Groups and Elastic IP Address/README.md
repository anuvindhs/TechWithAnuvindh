[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# AWS Security Groups and Elastic IP Address

**What is Security Groups and Elastic IP Address**
-   Security Groups - is like a firewall in the cloud that has set rules what traffic is allowed.
-   Elastic IP Address - is a static IP address that one can assign to AWS resources.

**What is it used for?**

-   Security Groups - controlling traffic either inbound or outbound for applying security to the network.
-   Elastic IP Address - Use a fixed IP address to assign to resources for easier access to users.

**Examples:**

-   Security Groups - Allowing port 80 and port 443 to a web server.
-   Elasic IP Address - Web Hosting, Allowing or Denying traffic to services

**Key Features**
-   Security Groups - Rules can be configured based on protocols and IP address.
-   Elastic IP address - Provide consistent public endpoint for applications.

**How EC2 Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowSecurityGroupWork.png
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowElasticIPAddressWorks.png)

**Benefits**
-   Security Groups - prevent unauthorized access by restricting network access.
-   Elastic IP Address - Offers flexibility in how to manage network resources.

**Use cases**
-   Security Groups - Add roles and rules instance like Web Server and Database.
-   Elastic IP Address - hosting applications like web servers that needs a consistent public IP address.

**Integration**
-   Use Elastic IP address and VPC Security Groups with rules to filter incoming traffic.

**Getting Started**
-   Security Groups - limit security grous and enforce least privilage acces.
-   Elastic IP Address - allocate an Elastic IP address before using it as it incurs a cost.

**Best Practices**
-   Security Groups - restrict inbound access to required IP address and port.
-   Elastic IP Address - Use DNS names instead of EIPs if possible.

**Challenges and Solutions**
-   Security Groups - Optimize your VPC(Virtual Private Cloud) security groups to bypass its limitations.
-   Elastic IP Address - Incurs costs, manage and release unused IP address and creating automated release process.

**Pricing overview**
-   Security Groups - No additional cost.
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/ElasticIPPricing.png)

**Case Studies**
-   Security Groups - Control traffic to resources by associating it to subnets.
-   Elastic IP Address - High availability for web servers.

**Conclusion**
-   Both are important for managing and securing cloud-based infrastructure.