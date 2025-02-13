[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# SES (Simple Email Service) and SNS (Simple Notification Service)

**What is SES and SNS?**
-  SES is a cloud based email service that allows one to send and receive emails.
-  SNS is a notification and messaging service that sends messages to recipients or systems.

**What is it for?**

-   SES - Allows one to configure an email service to send and receive messages.
-   SNS - Send notifications and messages to using different services that also has SMS option to be sent to customers

**Examples:**

-   SES - sending emails like marketing offers, communication letters, and alerts.
-   SNS - Monitoring to setup alerts, broadcast and event notifications, Mobile Push notifications.

**Key Features**
-   Allows publishers to send messages to specific topics
-   Message fanout that sends a message to multiple subscribers
-   Supports mutiple protocols
-   Message filtering

**How SES and SNS Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowSESSNSWorks.png)

**Benefits**
-   Bulk messaging, competitive per use pricing, active monitoring of metrics

**Use cases**
-   Application monitoring to alert of critical events, Mobile app notifications, Automated workflows.

**Integration**
-   Configure AWS SNS notifications for Amazon SES to notify bounces and delivers it through SNS.   

**Getting Started**
-   SES - Setup SES account, Grant programmatic access (IAM), download AWS SDK to use SES APIs.
-   SNS - Create a topic using SNS console then enable encryption.

**Best Practices**
-   Implement least privilege access to different permissions for specific tasks.

**Challenges and Solutions**
-   Lack of visibility into account inventory - Centralize with IAM Identity Centre or integrate with Active Directory.

**Pricing overview**
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/SESPricing.png)
![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/SNSPricing.png)

**Case Studies**
-   SES - Automate transactional messages, Globally deliver marketing emails
-   SNS - Push notifications, Distributed system architecture.

**Conclusion**
-   AWS SES and SNS is a suite of powerful services to handle messaging and communication needs.
