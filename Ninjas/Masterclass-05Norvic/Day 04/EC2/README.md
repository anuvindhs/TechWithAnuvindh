[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# AWS EC2 (Elastic Compute Cloud)

**What is EC2?**
-   service that allows the creation of virtual machines or computers to run applications in the cloud.

**What is it for?**

-   gives one the ability to use computer instances over the cloud to run applications without needing physical hardware.

**Examples:**

-   Website hosting and applications, Game servers, Disaster recovery

**Key Features**
-   Scalability - launch up or down mutiple instances.
-   Auto-Scaling - Adjust automatically the number of instances.
-   Storage options - optimized storage for intensive tasks.
-   Instance configurations - configure instances with specific resources.
-   AWS IAM roles - Provide access management for instances.
-   Operating System options - Choose from various operating systems.

**How EC2 Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowEC2Works.png)

**Benefits**
-   Highly reliable and secure. Also provides Flexibility.

**Use cases**
-   Hosting websites, Running batch jobs, Hosting development environments

**Integration**
-   Works with Amazon S3 to store data.
-   Works with VPC to create Virtual Private Clouds.

**Getting Started**
-   Create and login to your AWS Account by going to aws.amazon.com
-   Identify the instance type like EC2 and use the Dashboard to launch instance and create your virtual machine.
-   Configure instance by creating firewall rules and choosing storage options.

**Best Practices**
-   Regularly backup using Amazon EBS snapshots.
-   Set TTL for applications to 255.
-   Manage access by creating IAM profiles.

**Challenges and Solutions**
-   Connectivity problems - Check network settings and make sure it is correct.
-   Slow performance - Use Autoscaling to add or remove instances based on demand.

**Pricing overview**
-   Pay per compute by the hour or second(minimum of 60 seconds) with no commitments. 
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/EC2%20Pricing.png)

**Case Studies**
-   Social Media - develop a social media platform and data analytics.
-   Web Servers - Host stateless web servers.

**Conclusion**
-   EC2 allows users to develop and deploy applications faster with fewer hardware costs.
