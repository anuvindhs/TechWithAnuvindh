### What is ELB  
AWS service that automatically distributes incoming application traffic across multiple targets, such as EC2 instances, containers, and IP addresses, to ensure high availability and performance.  

Application Load Balancer (ALB)  -HTTP/HTTPS
  
Network Load Balancer (NLB)- For high-performance, high-throughput TCP traffic with low latency and millions of requests,

Classic Load Balancer (CLB)- The original load balancer that supports HTTP, HTTPS, and TCP protocols but with simpler functionality

### where to use     
Web Applications: Distribute web traffic evenly across multiple web servers.  

High Availability Architectures: Achieve high availability by distributing traffic across resources in multiple Availability Zones.  

Containerized Applications: Integrate with ECS (Elastic Container Service) or EKS (Elastic Kubernetes Service) to automatically route requests to container instances.  

Microservices Architectures: Route traffic based on different service types within an application.  

Disaster Recovery: Distribute traffic across multiple regions to improve fault tolerance  

 ### how to use  
 Create a Load Balancer: In the AWS Management Console, create an ELB, choose the appropriate load balancer type (ALB, NLB, CLB), and configure its subnets and security groups.  

Configure Target Groups: Define the target groups where the ELB will forward traffic (such as EC2 instances or Lambda functions), and set up health checks to ensure traffic is only sent to healthy targets.  

Set Up Listeners: Configure ELB listeners to receive client requests based on specified protocols (HTTP, HTTPS, TCP, etc.) and forward requests to the target groups.  

Adjust Routing Rules: In ALB, configure routing rules to send traffic to different target groups based on request attributes like URL paths or hostnames.  

Monitor and Scale Automatically: Use CloudWatch to monitor ELB performance and adjust traffic distribution and target instance scaling as needed.  


 
  ### Any note  
High Availability,Auto Scaling
