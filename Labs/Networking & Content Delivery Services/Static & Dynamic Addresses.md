## Internet Protocols - Static and Dynamic Addresses

<img width="867" height="569" alt="image" src="https://github.com/user-attachments/assets/d93f864a-17e5-4a9d-b154-3f9ca35a3ef6" />

**Overview**

In this lab, I will try to enable Elastic IP Addresses. This is done to keep a consistent IP Address even if an EC2 Instance is turned off or restarted.
Elastic IP Addresses keep the same public address even if anything happens to the EC2 Instance.

To begin with, I logged into the AWS Management Console and searched for EC2. I entered EC2 Instance and viewed the current Instances available.
<img width="1365" height="644" alt="Screenshot 2025-12-11 154555" src="https://github.com/user-attachments/assets/79d54504-586f-4dfa-8546-21709579a61c" />
<img width="1365" height="648" alt="Screenshot 2025-12-11 154617" src="https://github.com/user-attachments/assets/f2caa731-5101-41f0-9568-ffc2144797df" />

I then launched an Instance using an AMI and additional details.

<img width="1364" height="646" alt="Screenshot 2025-12-11 155031" src="https://github.com/user-attachments/assets/c5d06d5f-188b-41f8-9736-6806fc98178e" />
<img width="1365" height="645" alt="Screenshot 2025-12-11 155324" src="https://github.com/user-attachments/assets/695f31f0-10ed-4edd-991f-77a69433adfc" />

After launch, waited to for the Instance state to change to running. I then noted the public and private IPV4 address.

<img width="1365" height="645" alt="Screenshot 2025-12-11 155346" src="https://github.com/user-attachments/assets/a0fe5583-0ae1-4463-bf85-18b8222e93bb" />

Then I stopped the Instance , and noted the IPV4 Addresses when stopped. 

<img width="1365" height="646" alt="Screenshot 2025-12-11 155435" src="https://github.com/user-attachments/assets/1b8a8554-bec0-411d-8b67-9caea819d1ea" />
<img width="1363" height="646" alt="Screenshot 2025-12-11 155716" src="https://github.com/user-attachments/assets/56188d5d-7158-4df4-a4e5-840f8feb8ba8" />

I started the Instance again, and in the process I noted the public and private IPV4 Address.
I noted the changes to the public and private IPV4 Address to the Instance before and after stopping.

<img width="1365" height="644" alt="Screenshot 2025-12-11 155806" src="https://github.com/user-attachments/assets/e9181502-4887-42dd-a2f2-9ed77475b872" />

To ensure that the public IPV4 Address stays the same, I will have to enable an Elastic IP Address. I created the Instance , thenn associated  the Instance to the EC2 Instance i created earlier.
<img width="1365" height="646" alt="Screenshot 2025-12-11 160104" src="https://github.com/user-attachments/assets/f624877c-ae47-4b88-a7c7-cc1d91f09ca7" />
<img width="1365" height="646" alt="Screenshot 2025-12-11 160124" src="https://github.com/user-attachments/assets/e4308d15-564d-445f-95cf-14fa3bc308d9" />
<img width="1365" height="645" alt="Screenshot 2025-12-11 160655" src="https://github.com/user-attachments/assets/a95bb7ef-9ac5-414d-8276-4daebabddd1c" />
<img width="1365" height="645" alt="Screenshot 2025-12-11 160708" src="https://github.com/user-attachments/assets/0c0780b7-e2b8-416b-a6cb-2aebf4fc42ec" />

I then went back to EC2 and checked into the test instance to check the public and private IP Address. 
The public IP Address had changed to 100.22.46.65. This shows that Elastic IP Address works and is associated properly with the EC2 instance.

<img width="1365" height="643" alt="Screenshot 2025-12-11 160840" src="https://github.com/user-attachments/assets/2846c645-44a9-4bd8-ad8a-d94884807332" />



