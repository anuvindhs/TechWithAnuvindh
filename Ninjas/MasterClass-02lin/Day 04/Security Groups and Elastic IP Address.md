### What is security group and elastic ip 

A security group functions like a virtual firewall for your instances in AWS. It controls inbound and outbound traffic to and from your instances based on rules you define. You can configure security group rules to allow specific IP addresses, HTTP, or SSH access to your instances. For example, you can set a rule to allow only a certain range of IPs to access your instance via SSH, or to allow only HTTP traffic.  

An Elastic IP is a static public IP address provided by AWS for your EC2 instances. Unlike regular public IPs that change when instances are stopped and started, an Elastic IP remains fixed, meaning it doesn't change if you restart or stop your instance. This allows for a stable connection to your resources, making it easier to manage external access, especially in high-availability or disaster recovery scenarios.  

### where to use   

Used for controlling network traffic to EC2 instances in AWS :managing access to instances via protocols like SSH, HTTP, and HTTPS.
Can be used in conjunction with load balancers, RDS instances, or other AWS resources.
  

Used when you need a persistent, fixed public IP address that doesn't change.  


 ### how to use   
 
 Create and configure security groups in the AWS Management Console.  

 Allocate an Elastic IP via the AWS Management Console,Associate the Elastic IP with an EC2 instance OR reassign to another instacnes 


  ### Any note