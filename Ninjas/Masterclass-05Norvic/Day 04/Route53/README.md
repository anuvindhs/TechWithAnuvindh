[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# Route 53

**What is Route 53?**
-  AWS Route 53 is a DNS (Domain Name System) service to route traffic to website locations.

**What is it for?**

-   It translates readable websites to IP addresses to direct users to connect to websites easily.

**Examples:**

-   Website hosting, Domain registration, Traffic routing

**Key Features**
-   Domain registration - register domain names for your website or web application.
-   DNS routing - routes internet traffic to the resources of your domain.
-   Health Checking - monitor health of resources to verify availability.
-   DNS Firewall - protects DNS queries by fitering outbound traffic.

**How Route 53 Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/Route53Works.png)

**Benefits**
-   High availability, Cost-effective, Reliability, and scalability.

**Use cases**
-   Manage network traffic globally, build highly available applications

**Integration**
-   Integrated with AWS CloudTrail to capture information and send it to route 53 API.

**Getting Started**
-   Register domain names, then configure DNS routing, and setup health checks.

**Best Practices**
-   Use alias instead of CNAME records to improve performance.

**Challenges and Solutions**
-   Slow DNS propagation - Ensure to get certificates after successful propagation.

**Pricing overview**
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/route53pricing.png)

**Case Studies**
-  Managing global AWS local zones applications with Route 53 Geoproximity routing.

**Conclusion**
-   AWS Route 53 is a reliable and cost effective way to route end users to internet applications.
