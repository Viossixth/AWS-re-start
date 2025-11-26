## Building a DB Server 

Goal for the lab

<img width="887" height="444" alt="Screenshot 2025-11-24 145040" src="https://github.com/user-attachments/assets/efb7dede-d399-4e28-aceb-dc4d5577b419" />

Task 1: Setting Up Database Security
First, you'll create a security group that lets your web server talk to your RDS database. Go into the VPC console, create a new security group called "DB Security Group" in the Lab VPC, and add an inbound rule for MySQL/Aurora on port 3306. The key thing here is setting the source to your Web Security Group, which means only EC2 instances with that security group can access the database.

<img width="1365" height="643" alt="Screenshot 2025-11-24 230439" src="https://github.com/user-attachments/assets/06fb3716-8712-4590-96c5-b5bb5d7de19d" />

Task 2: Configuring Database Subnets
Next, you'll set up a DB subnet group that tells RDS which subnets it can use. Head to the RDS console and create a subnet group called "DB Subnet Group" in the Lab VPC. You need to add subnets from at least two availability zones, so select the first two zones and choose the 10.0.1.0/24 and 10.0.3.0/24 subnets (Private Subnets 1 and 2).

<img width="1365" height="645" alt="Screenshot 2025-11-24 231136" src="https://github.com/user-attachments/assets/0d9fcc56-a94a-4293-8b70-a9a39e456182" />


Task 3: Launching the RDS Database
Now you'll create the actual database. In the RDS console, create a new MySQL database using standard create mode. Choose the latest MySQL version and pick the Dev/Test template with Multi-AZ deployment (this creates a primary database that automatically replicates to a standby in another availability zone). Name it "lab-db" with username "main" and password "lab-password". Use a db.t3.medium instance with general purpose SSD storage. Connect it to the Lab VPC and attach the DB Security Group you created earlier. Remove the default security group. Create an initial database called "lab" and disable enhanced monitoring and automated backups to speed things up. Once you hit create, wait about 4 minutes for it to deploy, then grab the endpoint URL and save it somewhere.

<img width="1365" height="644" alt="Screenshot 2025-11-24 232617" src="https://github.com/user-attachments/assets/d534578f-f528-481b-ab54-c734e5289ec8" />

Task 4: Testing the Database Connection
Finally, you'll test everything by connecting a web application to your database. Open the WebServer IP address in your browser, click the RDS link in the app, and enter your database endpoint, database name (lab), username (main), and password (lab-password). The app will populate an address book using your RDS database, and you can add, edit, or remove contacts to see that the data is being stored and automatically replicated across both availability zones.

<img width="1365" height="648" alt="Screenshot 2025-11-24 235239" src="https://github.com/user-attachments/assets/d6fb7916-5265-4261-a21f-06a01fb07b5e" />
