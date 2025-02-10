## **Progress and Activities**

### 3-Tier Application

A 3-tier application is an architecture for an application that is split into three logical layers, each with a specific function that operates independently but interacts with another to process user requests.

 <img src="Assets\pic1.png" alt="pic1" width="500">

1. **Presentation Layer (Client Tier)**
   - The user interface (web browser, mobile apps) where users interact with the application.
   - Uses HTML, CSS, JavaScript, and related frameworks like React, Angular, or Vue.js.

2. **Logic Layer (Application/Business Tier)**
   - This layer processes user requests (for authentication, payments, data validation) by executing the business logic.
   - Uses PHP, Java, Python, Node.js, .NET, etc.

3. **Data Layer (Database Tier)**
   - The data layer stores and retrieves application data (user credentials, transaction records, product catalog).
   - Uses MySQL, PostgreSQL, MongoDB, SQL Server, etc.

### 3-Tier Applications Are Used For:
- Web applications (e.g., e-commerce websites, banking portals).
- Enterprise applications (e.g., CRM, ERP systems).
- Mobile applications (where APIs connect the mobile user interface to backend services).
- Cloud-based applications (e.g., SaaS products, online collaboration tools).

### Benefits of 3-Tier Architecture:
- **Scalability** – Each layer can be scaled independently on demand.
- **Security** – Data is processed separately in the logic and data layers, avoiding data leakage.
- **Maintenance** – Updates and debugging are easier due to the modular structure.
- **Flexibility** – Different technologies can be used for each layer.

### Types of Architecture:

 <img src="Assets\pic2.png" alt="pic2" width="500">

#### Monolithic Architecture:
Deploying all three layers (Presentation, Logic, and Data) of a 3-tier application on a single EC2 instance is not recommended.

1. **Scalability Issues:**
   - Each layer (Presentation, Logic, and Data) has different resource demands. For example, the data layer (database) might require more CPU and memory resources, while the presentation layer (web server) may require more bandwidth. If all layers are on one instance, it becomes challenging to scale them independently based on their specific needs.

2. **Performance Degradation:**
   - The layers might compete CPU and memory resources if dealing with high volume or complex requests, which can cause performance bottlenecks and slow response times.

3. **Security Risks:**
   - Without separating the layers, the application is more vulnerable to an attack as credential, transactional data stored in the database can be potentially exposed.

4. **Added Maintenance:**
   - Updates or changes to one layer which require restart can impact the other layer. Handling the different technologies for each layer is also challenging.

5. **Cost Inefficiency:**
   - Under-utilization of CPU and memory resources for each layer can be wasteful.

#### 3-Tier Architecture:
In a 3-tier architecture, components are separated into distinct layers each running on a separate EC2, for better scalability, flexibility, security, maintenance, and performance.

#### Serverless 3-Tier Architecture:
In a serverless 3-tier architecture, AWS managed serverless services such as S3, Lambda, and DynamoDB handle scaling and infrastructure management automatically for the 3 layers. This can be a cost-effective solution as you pay only for the actual usage, not for provisioning or managing infrastructure.

---

### Cloud Deployment and Validation Cycle
This process is followed by cloud engineers when deploying, testing, and validating cloud-based applications or environments. The process ensures that the environment is correctly configured, functional, and meets the requirements before moving to production.

1. **Research:**
   - Gather information to ensure best practices are followed using trusted resources. Review official documentation, such as Git repositories, cloud provider guides, or community sources, to gather the correct steps for setting up the environment or application. Identify any prerequisites or dependencies that need to be met before deployment (e.g., operating systems, libraries, or configurations).

2. **Test:**
   - Deploy the cloud infrastructure including cloud instances such as AWS EC2 and install the necessary software stack such as LAMP (Linux, Apache, MySQL, PHP). Configure networking, security settings (firewalls, security groups). Automate the deployment process using Infrastructure as Code (IaC) tools such as Terraform where applicable.

3. **Validate:**
   - Perform functionality checks of the deployed infrastructure and software for the application. For example, open the website in a browser to check if the web server and database are interacting correctly for database queries and meeting requirements. Verify all configurations such as permissions, correct paths are correct and secure.

4. **Repeat:**
   - Troubleshoot any problems such as misconfigurations, performance bottlenecks, and security vulnerabilities identified in validation. Change or optimize configurations before redeploying the refined environment. Performing load tests or scalability checks before passing it through production.

---

### 3-Tier Application Lab Part 1

- **Launch EC2.**
 <img src="Assets\pic3.png" alt="pic3" width="500">
  <img src="Assets\pic4.png" alt="pic4" width="500">

- **Connect to EC2 through terminal using SSH key.**

 <img src="Assets\pic5.png" alt="pic5" width="500">

- **Confirm Git is available in EC2:**  
  Command: `git -v`

- **Update ubuntu:**  
  Command: `sudo apt update -y`

   <img src="Assets\pic6.png" alt="pic6" width="500">

- **Install Apache web server:**  
  Command: `sudo apt install apache2 -y`

 <img src="Assets\pic7.png" alt="pic7" width="500">

- **Validate Apache 2 has installed successfully.**

 <img src="Assets\pic8.png" alt="pic8" width="500">

- **Install WordPress dependencies:**  
  Command: `sudo apt update`  
  `sudo apt install apache2 ghostscript libapache2-mod-php mysql-server php php-bcmath php-curl php-imagick php-intl php-json php-mbstring php-mysql php-xml php-zip`

   <img src="Assets\pic9.png" alt="pic9" width="500">

- **Validate MySQL Installation:**
Validate MySQL has been installed successfully. Change to root because checking for database.
Command:
`sudo su`
`mysql -v`

<img src="Assets\pic10.png" alt="pic10" width="500">

- **Create Installation Directory and Download WordPress:**
Create the installation directory and download the file from WordPress.org. 
Command:
`sudo mkdir -p /srv/www`
`sudo chown www-data: /srv/www`
`curl https://wordpress.org/latest.tar.gz | sudo -u www-data tar zx -C /srv/www`

<img src="Assets\pic11.png" alt="pic11" width="500">

- **Validate WordPress Installations:**
Validate WordPress has been installed to the correct file directory. 
Command:
`cd /srv/www`
`ls`

<img src="Assets\pic12.png" alt="pic12" width="500">

- **Configure Apache for WordPress:**
Configure Apache to point the WordPress site as the main index. Change directory and create file. 
Command:
`sudo nano /etc/apache2/sites-available/wordpress.conf`

<img src="Assets\pic13.png" alt="pic13" width="500">

Inside the file, add the following configuration: 
Command:
<VirtualHost *:80>
    DocumentRoot /srv/www/wordpress
    <Directory /srv/www/wordpress>
        Options FollowSymLinks
        AllowOverride Limit Options FileInfo
        DirectoryIndex index.php
        Require all granted
    </Directory>
    <Directory /srv/www/wordpress/wp-content>
        Options FollowSymLinks
        Require all granted
    </Directory>
</VirtualHost>

<img src="Assets\pic14.png" alt="pic14" width="500">

Enable the Site
Command:
`sudo a2ensite wordpress`

Enable URL Rewriting
Command:
`sudo a2enmod rewrite`

Disable the Default "It Works" Site
Command:
`sudo a2dissite 000-default`

<img src="Assets\pic15.png" alt="pic15" width="500">

Restart Apache 2
Command:
`sudo systemctl reload apache2`

<img src="Assets\pic16.png" alt="pic16" width="500">

### Stopping and Starting EC2 Instance via PowerShell

**Stopping instance:**
Command: 
`aws ec2 stop-instances --instance-ids [enter instance id here]`

<img src="Assets\pic17.png" alt="pic17" width="500">

**Starting instance:**
Command: 
`aws ec2 start-instances --instance-ids [enter instance id here]`

<img src="Assets\pic18.png" alt="pic18" width="500">
