[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# CloudFront

**What is CloudFront?**
-  AWS service that delivers content to websites faster by distributing data from server locations near the users who are accessing it

**What is it for?**

- It is a faster way of delivering website content to where users are accessing it by getting data from the main server to a nearby server

**Examples:**

-   Wesbites like E-Commerce sites, Video Streaming Service, Software updates.

**Key Features**
-   Availability - Redundancy by supporting multiple origins for backend architecture.
-   Security - Protection against network and application layer attacks.
-   Realtime metrics and logging - Integrated with CloudWatch and provides realtime logs.
-   Continous deployment - Deploy two separate identical environment safely.

**How CloudFront Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/CloudFrontWorks.png)

**Benefits**
-   Low Latency by caching content at locations close to users
-   High transfer speeds to deliver content quickly by using AWS backbone.

**Use cases**
-   Fast and secure websites, Stream live and on-demand video, distribute patches and updates.

**Integration**
-   Integrates with EC2, S3, Application Load Balancers or any custom HTTP origin.

**Getting Started**
-   Create an S3 bucket then upload content in the bucket then create a CloudFront distribution that uses S3 origin with OAC.

**Best Practices**
-   Analyze ussage patterns and select the appropriate pricing tier. 
-   Regularly monitor and analyze AWS CloudFront costs.

**Challenges and Solutions**
-   Caching related issues - Analyze cache behaviors and align it with your content's caching requirements.

**Pricing overview**
-   ![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/CloudFrontPricing.png)

**Case Studies**
-   Full website delivery, Adaptive video streaming, API protection and acceleration.

**Conclusion**
-   AWS CloudFront delivers fast distribution of web content using a network of data centres providing low latency and performance.
