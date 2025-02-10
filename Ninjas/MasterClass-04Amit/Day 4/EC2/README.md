# **Amazon EC2: Scalable Cloud Computing**

## **Purpose**  
Amazon Elastic Compute Cloud (EC2) provides unlimited computing power in the cloud, allowing businesses to spin up to 750 virtual machines (instances) on demand. It offers customizable latest processors, storage, networking, and operating systems to meet diverse workload requirements without massive hardware investments upfront.

<img src="Assets\ec21.png" alt="ec21" width="500">

## **How It Works**  
AWS data centres host the EC2 which is accessible to the user from anywhere, providing the ability to customize on the fly.
1. **Instance Provisioning:**
   - Launch the instance.

   <img src="Assets\ec22.jpg" alt="ec22" width="500">

   - Choose an Amazon Machine Image (AMI) to define the operating system and pre-configured software.

   <img src="Assets\ec23.jpg" alt="ec23" width="500">

   - Select an instance type (CPU, memory, storage, and network capacity).

   <img src="Assets\ec24.jpg" alt="ec24" width="500">

   - Set up a key pair for secure instance access using public-private keys.

   <img src="Assets\ec25.jpg" alt="ec25" width="500">

2. **Configure Network Settings:**
   
   - Choose the network settings like the VPC and subnet for communication with the instance.

   <img src="Assets\ec26.jpg" alt="ec26" width="500">

3. **Configure Security Group:**

   - Create or select default security group which acts as a firewall for the instance. Define inbound and outbound rules to control network traffic.

   <img src="Assets\ec27.jpg" alt="ec27" width="500">

4. **Storage and Deployment:**
   - Configure storage options (EBS volumes).

   <img src="Assets\ec28.jpg" alt="ec28" width="500">

   - Launch the instance in a Virtual Private Cloud (VPC) and connect using SSH/RDP.
5. **Application Deployment:** 
   - Deploy applications on the instance.
6. **Scaling & Optimization:**
   - Use Auto Scaling to match resource allocation with demand.
   - Monitor performance using Amazon CloudWatch to optimize costs and resources.



## **Features & Benefits**  
- **Customizable Instances:** Tailor compute resources to exact workload requirements minimizing unnecessary running costs(OpEx).
- **Auto Scaling:** Scale resources up or down minimizing upfront hardware investment (CapEx).
- **Cost-Effective:** Pay-as-you-go pricing and Spot Instances for significant savings.
- **Security:** Built in AWS Nitro System to the instance ensures data is secure.
- **Fast Provisioning:** Launch virtual machines within minutes with a 99.99% SLA uptime guarantee.
- **Global Reach:** Operate across multiple regions and Availability Zones for enhanced resilience.



## **Use Cases**  
- Hosting websites, web applications, and APIs.  
- Running custom or off-the-shelf applications (e.g., CRM).  
- Processing data-intensive workloads like video rendering or scientific simulations.  
- Training machine learning models and inference tasks.  
- Gaming servers and edge computing for IoT data aggregation.  
- Scalable video streaming (e.g., Netflix).  
- Deploying containerized applications (e.g., Docker, Kubernetes, microservices).



## **Pro Tips**  
1. **Optimize Costs:** Use Reserved Instances for predictable workloads to save up to 72%.  
2. **Automate Provisioning:** Utilize AWS CLI or Terraform to streamline deployments.  
3. **Set Alerts:** Use CloudWatch for critical metrics like CPU, memory, and disk usage.  
4. **Enhance Performance:** Choose the latest generation instances for better efficiency.  
5. **Secure Access:** Rotate SSH/RDP keys periodically and restrict network access with security groups.  




## **Common Issues**  
- **Cost Management:** Unused or forgotten instances contribute to cost creep.  
- **Connection Errors:** RDP timeout errors when connecting to instances.  
- **Billing Limits:** Instances may terminate or stop unexpectedly if billing limits are exceeded.


## **Pricing**  
- **Pay-As-You-Go:** Competitive pricing based on usage.  
- **Discounts:** Spot pricing and Reserved Instances provide significant cost reductions.
