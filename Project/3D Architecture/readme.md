![WhatsApp Image 2025-12-04 at 14 58 27](https://github.com/user-attachments/assets/48e0a27f-4575-471d-a114-64e7b6adb5a1)


## Project Overview 

The aim of this project was to design infrastructure for an ecommerce application or website which would have 3D Objects of their inventory. AWS services should be used for security, monitoring, performance and scalability. An infrstaructure diagram was drawn showing the various services used and the logical flow of information. A Project brief was written up explaining why each service was chosen and it's function, how the architecture meets the five requirements and any design trade-offs or challenges faced.

## Why each service was chosen

**Frontend**

The frontend refers to the client-side of the application, focusing on user experience and interface. It's what users interact with directly more like the face of the app.
* Route 53: Domain name system (DNS) management for routing users to the application, providing high availability and scalability. Think of it like a phonebook of internet. It helps users find your app by translating domain names into IP addresses.
* CloudFront: Content delivery network (CDN) for distributing static assets, reducing latency, and improving user experience. Imagine a network of caching servers around the world, storing copies of your website's static files, so users get faster access no matter the location.
* Amplify Hosting: Managed hosting for web applications, providing automated deployment, SSL/TLS, and integration with other AWS services. It's like having a hosting service that takes care of all the technical details, so you can focus on building your app.

**Backend**

The backend refers to the server-side of the application, handling business logic, database interactions, and API integrations. Basically this is where the magic happens.
* App Runner: Containerized application hosting, simplifying deployment and scaling of containerized applications. It's more of like having a managed platform for running your containerized apps, without worrying about the underlying infrastructure.
* Lambda: Serverless compute for handling small, event-driven tasks, reducing operational overhead. Think of it like a service that runs your code only when needed, without requiring server management.



**Storage**

Storage refers to the services used to store and manage data. 
* S3 (3D assets + static files): Object storage for hosting static files, providing durability, scalability, and high availability. It's like having a massive, secure hard drive in the
  cloud, where you can store and serve files.

**Databases**

Databases are specialized storage services for structured data.
* DynamoDB (catalog): NoSQL database for handling high-traffic catalog data, providing low latency and scalability. It's designed for fast, efficient data retrieval and storage.
* RDS PostgreSQL (orders / users): Relational database for managing orders and user data, providing ACID compliance and SQL querying capabilities. It's a managed database service, handling the underlying infrastructure, so you can focus on your data.

**Performance**

Performance services focus on optimizing application speed and efficiency.
* ElastiCache Redis: In-memory caching for improving application performance, reducing database load, and enhancing user experience. It's like having a super-fast cache layer, storing frequently accessed data.
* SQS + Lambda workers: Message queuing and processing for handling asynchronous tasks, decoupling application components, and improving scalability. It's like having a message broker, handling task queues and processing, so your app can focus on other things.

**Security**

Security services protect the application and its data from threats and vulnerabilities.
* WAF: Web application firewall for protecting against common web exploits and vulnerabilities. It's like having a security guard, monitoring and blocking malicious traffic.
* Shield: DDoS protection for safeguarding against distributed denial-of-service attacks. It's like having a shield, protecting your app from overwhelming traffic.
* KMS: Key management service for encrypting sensitive data and managing encryption keys. It's like having a secure key vault, protecting your encryption keys.
* Secrets Manager: Secrets management for securely storing and retrieving sensitive information, such as database credentials. It's like having a secure password manager, storing and retrieving secrets.

**Monitoring**

Monitoring services track application performance, errors, and security issues.
* CloudWatch: Monitoring and logging service for tracking application performance, errors, and security issues. It's like having a dashboard, showing real-time insights into your app's health.
* Cost Explorer: Cost management tool for analyzing and optimizing AWS costs, ensuring efficient resource utilization. It's like having a financial advisor, helping you optimize your AWS spending.



## Design trade-offs or challenges

**Using App Runner vs. ECS or Lambda for Compute**

App Runner provides simplified deployment, autoscaling, and HTTPS, reducing operational burden. The trade-off is reduced infrastructure control and higher costs for long-running
workloads. It prioritizes developer speed over deep customization.

**DynamoDB + RDS Combination**

Using DynamoDB for catalog data and RDS PostgreSQL for transactional workloads improves performance and reliability. The trade-off is increased operational complexity, duplicated data models, and the need for careful consistency management.

**CloudFront + Amplify Hosting**

Amplify Hosting simplifies frontend deployment, while CloudFront provides global caching. The challenge is managing cache invalidation so users do not see outdated content. This requires deliberate cache behaviors and versioning strategies.

**High Availability vs. Cost**

Multi-AZ RDS, autoscaling compute, global CDN distribution, and caching layers improve uptime and performance, but they significantly increase cost. Teams must balance reliability with budget constraints.

**Introducing SQS and Lambda Workers**

SQS and Lambda provide reliable asynchronous processing. The trade-off is additional moving parts (queues, DLQs, retry logic). Teams must ensure idempotency and message integrity to avoid duplicate order processing.


## Challenges and Resolutions

This project was very straight-forward as it encompasses all of the knowledge of the AWS ecosystem i have so far, so majority of the work was to reflect and do some further research in order to have accurate information. I was responsible for the second part of the write up where i have to discuss how the chosen services meet the five requirements of High availability, scalability, Performance, Cost Optimization and Security. All I had to do was recollect my knowledge and do some research on each service to ensure accuracy and that i understand the core concept of each service when I write the write up. In terms of time management, I was a bit unwell the week of this project as well as having to fix my AWS re/Start repository and Canvas tasks but I separated the work well, gave myself time to rest and did some well when I felt better. I managed to complete all the tasks in time, and was happy with my effort as well as my teams found it satisfactory.

**The Project write up is available at the following link**

https://github.com/Viossixth/AWS-re-start/blob/main/Project/3D%20Architecture/Project%202.pdf
