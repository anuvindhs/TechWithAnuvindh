[back](/Ninjas/Masterclass-05Norvic/Day%2004/README.md)

# Lambda

**What is Lambda?**
-  Service that lets one run code in the cloud without needing to setup servers.

**What is it for?**

-   Lambda executes code functions when an event is triggered.

**Examples:**

-   Trigger Lambda if a file is uploaded to S3, Execute a function if a new data is added to a database (RDS, DynamoDB).

**Key Features**
-   Versions - manage deployment with versions using beta testing for stable production version.
-   Lambda Libraries - Package libraries and other dependencies to reduce size of deployment.
-   Private networking - create a private network for resources like databse.
-   Function URL - add a dedicated HTTP(S) endpoint to a lambda function.

**How Lambda Works**

![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/HowLambdaWorks.png)

**Benefits**
-   No need to manage servers, automatic scaling, Pay as you go pricing.

**Use cases**
-  Credit card company used Lambda to save developer time thus improving speed to market and reducing cost by using serverless technology.

**Integration**
-   Build and API with Lambda integration

**Getting Started**
-   Developers write the code then pay only for execution time then upload code with simplified deployment for easy integration with other services.

**Best Practices**
-   Plan the deployment of the function code then use a keep alive directive to maintain connection. 

**Challenges and Solutions**
-   Limitation of a function run for 15 minutes - Break down processes into smaller ones.

**Pricing overview**
-   ![screenshot](/Ninjas/Masterclass-05Norvic/Day%2004/Assets/LambdaPricing.png)

**Case Studies**
-   Data processing, Web APIs, File Processing.

**Conclusion**
-   AWS Lambda is a serverless compute service which executes code, handle compute resources which is cost effective especially in application development.
