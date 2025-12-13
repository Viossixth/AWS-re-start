## Install and Configure the AWS CLI

<img width="915" height="384" alt="image" src="https://github.com/user-attachments/assets/47bf382b-a84c-43af-8cea-c5e51c166608" />


**Task 1**

To complete task 1, i logged into the AWS Management console, and searched for EC2. On the EC2 landing page, i looked for the instances button and clicked it.
I looked for the Publib IP Address of the running Instnace and copied it into a notepad. On the Vocareum labs page, I clicked on details and downloaded the ppk file. I used Putty to connect to the EC2 Instance using the username: EC2-User and the Public IP Address.

<img width="1365" height="647" alt="Screenshot 2025-12-13 200543" src="https://github.com/user-attachments/assets/f7152161-de57-46e5-8fd8-08c0fa382889" />
<img width="1365" height="644" alt="Screenshot 2025-12-13 200551" src="https://github.com/user-attachments/assets/b50267c8-871c-4f09-8bfd-c253caa63142" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 200608" src="https://github.com/user-attachments/assets/543c10ad-92da-4bc7-be5e-14a6743fb23a" />
<img width="1365" height="646" alt="Screenshot 2025-12-13 200630" src="https://github.com/user-attachments/assets/a5ede8ab-569e-4b27-8bf3-775cbdb335ba" />
<img width="1365" height="767" alt="Screenshot 2025-12-13 200652" src="https://github.com/user-attachments/assets/18788d85-7aff-490e-9429-ff6f5582c9d8" />

**Task 2**
 
 In task 2, I had to write the downloaded file into the current directory. After this, I unzipped the installer and ran the program to confirm installation. The AWS CLI ran and gave me the expected output, I then used the command "aws help" to ensure that it is working perfectly. 

<img width="1365" height="767" alt="Screenshot 2025-12-13 200958" src="https://github.com/user-attachments/assets/64c60891-fc86-4ce5-a282-d414578e8169" />
<img width="1365" height="767" alt="Screenshot 2025-12-13 201036" src="https://github.com/user-attachments/assets/82b63e7d-7e4d-465c-987f-502e0bfe65ca" />


**Task 3**

To complete Task 3 I returned to the AWS Management console and searched for IAM. On the landing page, I clicked on users and found awsstudent. I clicked on the permissions tab and noted what I saw. 
I also went to the security credentials tab and to note of the access keys. I got the access keys from the Vocareum labs details section.

<img width="1365" height="645" alt="Screenshot 2025-12-13 201646" src="https://github.com/user-attachments/assets/4142acf5-4427-49bb-9702-5f53a047740c" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 202328" src="https://github.com/user-attachments/assets/88b4dc0a-56ed-4a25-9fa3-ebac4ce05893" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 202552" src="https://github.com/user-attachments/assets/1cc9ad23-815a-4cea-b684-7074bfecc114" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 202524" src="https://github.com/user-attachments/assets/e9ad29d7-5d91-4650-8b3f-b95a6dd7053f" />


**Task 4: Configure the AWS CLI to connect to your AWS Account**

In thsi task i had to configure the AWS CLI using the "aws configure" command. I then had to insert the access key, secret key, default region name and default output format. 

<img width="1364" height="647" alt="Screenshot 2025-12-13 203704" src="https://github.com/user-attachments/assets/5101de4b-cd09-4954-9f2a-fde3db32fa6f" />
<img width="1365" height="767" alt="Screenshot 2025-12-13 203735" src="https://github.com/user-attachments/assets/a094114d-15fa-4071-acd2-b0596e72c479" />

**Tasks 5:Observe IAM configuration details by using the AWS CLI**

In the last step I had to view the list of IAM users logged in, this is done to verify what I did in task 4. I used the " aws iam list-users" command and only one user appeared, the user I configured in task4.

<img width="1365" height="767" alt="Screenshot 2025-12-13 204152" src="https://github.com/user-attachments/assets/62db56b5-ad42-49c0-97cc-f39a9857b615" />

**Summary**

In this lab I gained experience with the AWS Command Line Interface, EC2 and IAM. I learnt how to connect to the ec2 using ssh (Putty) and downloading, unziping and running the aws cli. I learnt how to configure a user and confirm if the user is logged in.
This lab was helpful in gaining experience with IAM controls and permissions, learning how to quickly configure an aws cli and user.

