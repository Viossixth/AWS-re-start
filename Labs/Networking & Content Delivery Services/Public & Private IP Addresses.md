## Public and Private IP Addresses

<img width="813" height="532" alt="image" src="https://github.com/user-attachments/assets/551ba642-0e8c-4847-80b6-00e1b373f817" />

In this lab I explore public and private IP Addresses and gain experience trying to connect to them. To start this lab, I logged into the AWS Management Console and searched for EC2. 

<img width="1365" height="646" alt="Screenshot 2025-12-11 144059" src="https://github.com/user-attachments/assets/fc895d1c-f348-432c-b2ca-73181b6758c4" />

I looked up Instances on the left navigation menu on EC2 and clicked to see the instances available. I selected Instance A , went to the networking tab to note the IP Address and only found the private address. 
<img width="1365" height="645" alt="Screenshot 2025-12-11 145350" src="https://github.com/user-attachments/assets/64cc2d45-1155-48ed-8810-59bc7f732a0d" />

I then selected Instance B and went to the networking tab to note the details. Instance B has both a public and private IP Address.
<img width="1365" height="647" alt="Screenshot 2025-12-11 145458" src="https://github.com/user-attachments/assets/0a6ce48a-875d-4bef-9b40-cf647eda36cc" />

I then used Putty to connect to Instance B which has a public IP Address and used a ppk key.
<img width="1365" height="646" alt="Screenshot 2025-12-11 144400" src="https://github.com/user-attachments/assets/141451f1-77b6-4732-8abf-419846801773" />
<img width="1365" height="767" alt="Screenshot 2025-12-11 144435" src="https://github.com/user-attachments/assets/d84b4f88-a7a9-4a0f-9830-545a82bec7d3" />

After connecting, i then changed directories using the "cd ~/Downloads" command and then used the "chmod 400 labsuser.pem" to change user permissions to read only. I then tried to connect to Instance A through the IP Address i noted earlier. The connection was unsuccessful, due to it being a private IP Address.
<img width="1365" height="767" alt="Screenshot 2025-12-11 144626" src="https://github.com/user-attachments/assets/ad5ec691-b82a-43df-b456-e995d93f42ca" />


**Lessons**

I gained experience working with Putty as a connection tool for EC2 instances and EC2. I learnt that you can't connect to a private EC2 instance if you're outside the VPC.
I could connect to Instance B because it had a public IP Address but couldn't do so with Instance A because it had no Public IP Address. 
