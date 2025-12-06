## Application & Integration Services

In this section, I cover the Application & Integration Services offered by AWS. These services are Amazon AppFlow, Amazon EventBridge,Amazon Step Functions, Amazon Simple Workflow Service (SWF), AWS Health Dashboard, Amazon Simple Que Service (SQS) and Amazon Simple Notification Service (Amazon SNS). 

Amazon Appflow is an integration service that allows for simple data transfer between a client's AWS Ecosystem and other Software service vendors such as slack, Google Analytics and SalesForce and vice versa. It allows data transfer without having to manage or write any code.
Appflow allows simple intergration, highly scalable, data is kept secure and there is time efficiency benefit when using Appflow.

<img width="1354" height="600" alt="image" src="https://github.com/user-attachments/assets/0fe2f3f9-2695-407d-9266-074891fb38c2" />


Amazon EventBridge is a service that intergrates multiple applications or SaaS services by the exchange of events. EventsBridge helps in coordinating complex event driven relations between services or applications. It reduces the need for manual checking or integration.
Amazon EventBridge can send real time alerts, trigger Lambda's and react to business events.

<img width="1461" height="621" alt="eventbridge-content-filtering-1" src="https://github.com/user-attachments/assets/8dcd079d-c133-42bb-876e-aaa462c1772d" />

Amazon Step Functions is an orchestration service using a visual workflow to coordinate multiple steps involving multiple application or services without writing any code, just managing the coordination logic.
Amazon Step Functions is used for Order processing workflows, data pipelines, ML model training, Approval workflows and ETL Automation. These are some scenarios where multiple steps and/or services are required.

<img width="1332" height="1000" alt="image" src="https://github.com/user-attachments/assets/e7fd703f-1fb1-4cbf-90a5-79faaa19e7bb" />


Amazon Simple Workflow is a service helping with orchestrating complex processes. It can recover from failures, track workflows and manage state of a workflows without any code. Amazon SWF is similar to a "to-do-list" , being able to track the state of a workflow and coordinate taks.
Amazon SWF is used for Order fillfulment, document processing, Video encoding and financial approval systems.

<img width="1000" height="364" alt="image" src="https://github.com/user-attachments/assets/73e057aa-29e3-45b4-af38-33a46327facf" />

Amazon Simple Queue Services is a managed message queing system helping tighlty couples microservices communicate to each other. It is fully managed , has good message durability and serverless. There are two types of queues, standard queue and First-In-First-Out .

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/ccd3048e-f37e-4e10-9cdf-a0a7888d8c97" />

Amazon Simple Notification Service is messaging solution from publishers to subscribers. It allows publishers to communicate to subscribers via HTTP/HTTPS, Email, SMS, Mobile Notifications or SQS Queues. It can send millions of messages per second, supports KMS for encryption, has good durability and retry logic.

<img width="1602" height="640" alt="image" src="https://github.com/user-attachments/assets/fde2e09f-e020-49cc-8689-9a97f6a22545" />

Amazon Simple Email Services is a platform that allows sending and reception of email securely in the cloud. It's a serverless service, built with reliability and scale in mnd. It is used for application transactions, marketing and notification emails by developers and businesses.

<img width="2360" height="912" alt="image" src="https://github.com/user-attachments/assets/9afb2028-404a-4f86-b7d8-be32d70fa257" />

Amazon MQ is a message brokerage service for Apache ActiveMQ and RabbitMQ.

<img width="974" height="485" alt="image" src="https://github.com/user-attachments/assets/b8a5e576-e25c-457c-966c-b04ebf7a7098" />

**Benefits**

* Scale with ease
* Simplify workflow orchestration
* Build resilient applications
* Ensure high availability

**Use cases**

* Automate security and IT functions.
* Automate ETL processes.
* Low latency event messaging
* Increase application reliability and scale.
