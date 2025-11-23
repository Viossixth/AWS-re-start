Introduction to Amazon EC2

Amazon EC2 is a web service that allows customers to provision servers known as instances. They can setup the instance accorsing to their predicted workload and has the ability to cater for future growth. This lab, showcases how an instance is setup. The following six steps are covered in this lab.

* Launch a web server with termination protection enabled

* Monitor Your EC2 instance

* Modify the security group that your web server is using to allow HTTP access

* Resize your Amazon EC2 instance to scale

* Test termination protection

* Terminate your EC2 instance

<img width="1062" height="564" alt="Screenshot 2025-11-23 211836" src="https://github.com/user-attachments/assets/ecf8116f-4e58-43b5-b95a-ccca7b656c61" />

Launching a webs server

To create a new instance, go to EC2 in the AWS Management Console.
<img width="1362" height="680" alt="Screenshot 2025-11-23 212413" src="https://github.com/user-attachments/assets/ed8c231d-3ec9-417c-9a3b-7c0aa1957d9b" />

Select Instances, on the left menu and click create instances on Page listing all instances. Choose a name for your instance and the AMI for your instance. An AMI is a template on which you can configure you're desired instance. Choose your instance type which determines the VCPU and Memory of your instance. Careful attention must be paid, to ensure the chose instance type corresponds with the type of workload your instance will do. For added security, a key pair can be used to encrypt and decrypt information. A security group should be configured after.

<img width="1363" height="678" alt="Screenshot 2025-11-23 212525" src="https://github.com/user-attachments/assets/f1417f71-1f84-47ad-ba90-5a84e59cb8da" />

<img width="1365" height="679" alt="Screenshot 2025-11-23 213128" src="https://github.com/user-attachments/assets/19f5ab7a-fb97-496b-94fb-f2a154e69337" />

To monitor the instance. view the instance from the instance page. Select the checkbox of the required instance , go to Actions , monitor and troubleshoot and get instance snapshot. Additionally you can go to the monitoring tab to check on monitoring metrics.
![i-056b6e5b1d9279f2e](https://github.com/user-attachments/assets/a0596d8c-1a18-48bb-9011-5c6d62d8aeef)

To access the web server, copy the IPV4 public address and insert it into a new tab. On the first attempt nothing could load.
<img width="1365" height="721" alt="Screenshot 2025-11-23 214449" src="https://github.com/user-attachments/assets/ddb08959-7f61-493a-b7d8-63e277d82c12" />

To solve this issue, Security group rules need to be changed. The inbound rules need to be changed.

<img width="1365" height="677" alt="Screenshot 2025-11-23 214438" src="https://github.com/user-attachments/assets/46e81f65-af26-4edb-be02-b400670ddbcd" />
<img width="1365" height="679" alt="Screenshot 2025-11-23 233342" src="https://github.com/user-attachments/assets/f448d7bb-6c10-46c1-b6de-1295ec195711" />







