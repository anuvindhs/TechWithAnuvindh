## **Progress and Activities**

### 3-Tier Application Lab Part 2

- **Edit configuration file adding own host name**

    Command: `sudo nano /etc/hosts`

     <img src="Assets\pic1.png" alt="pic1" width="500">
      <img src="Assets\pic2.png" alt="pic2" width="500">

- **Validate file has been modified correctly and restart the Apache server:**
git p
    Command: `cat /etc/hosts`
    Command: `sudo service apache2 restart`

      <img src="Assets\pic3.png" alt="pic3" width="500">

- **Configure Data Layer – MySQL Database**

    Command: `sudo mysql -u root`

    <img src="Assets\pic4.png" alt="pic4" width="500">

- **Create Database:**

    Command: `CREATE DATABASE wordpress;`

- **Create Username and Password:**

    Command: `CREATE USER <enterusername>@localhost IDENTIFIED BY '<enterpassword>';`

- **Give Permissions:**

    Command: 
    `GRANT SELECT,INSERT,UPDATE,DELETE,CREATE,DROP,ALTER`
    `ON wordpress.*` 
    `TO <enterusername>@localhost;`

    Command: `FLUSH PRIVILEGES;`
    
    Command: `quit`
    
    Command: `sudo service mysql start`

    <img src="Assets\pic5.png" alt="pic5" width="500">

- **Configure WordPress to Use the Database:**

Give user www-data privilege to copy the sample file wp-config-sample.php to the main file wp-config.php:
Command: 
`sudo -u www-data cp /srv/www/wordpress/wp-config-sample.php /srv/www/wordpress/wp-config.php`

<img src="Assets\pic6.png" alt="pic6" width="500">

Set the Database Credentials in the Configuration File:
Command:
`sudo -u www-data sed -i 's/database_name_here/<enterdatabase>/' /srv/www/wordpress/wp-config.php`
`sudo -u www-data sed -i 's/username_here/<enterusername>/' /srv/www/wordpress/wp-config.php`
`sudo -u www-data sed -i 's/password_here/<enterpassword>/' /srv/www/wordpress/wp-config.php`

Validate configuration of the file:
Command: 
`cat /srv/www/wordpress/wp-config.php`

<img src="Assets\pic7.png" alt="pic7" width="500">

Edit wp-config Configuration File with Salt Key
Command: 
`sudo -u www-data nano /srv/www/wordpress/wp-config.php`

<img src="Assets\pic8.png" alt="pic8" width="500">
<img src="Assets\pic9.png" alt="pic9" width="500">
<img src="Assets\pic10.png" alt="pic10" width="500">

Validate Database, User, and Privileges
Command: `SHOW DATABASES;`
Command: `SELECT user, host FROM mysql.user;`
Command: `SHOW GRANTS FOR '<username>'@'localhost';`

<img src="Assets\pic11.png" alt="pic11" width="500">

- **Open WordPress in Browser:**
<img src="Assets\pic12.png" alt="pic12" width="500">

Create an account. Choose a username and password that are different from your MySQL (database) credentials.

<img src="Assets\pic13.png" alt="pic13" width="500">

Login using the credentials.

<img src="Assets\pic14.png" alt="pic14" width="500">

In the WordPress Dashboard, customize the website.

<img src="Assets\pic15.png" alt="pic15" width="500">