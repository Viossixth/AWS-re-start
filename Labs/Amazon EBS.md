## Configuring and Working on Amazon Elastic Block Store (EBS)

<img width="813" height="235" alt="lab-scenario" src="https://github.com/user-attachments/assets/37882e40-444a-4eb2-bf21-f6289f329f46" />

To get started, i logged into the AWS Management Console and searched for EC2. On the left navigation menu, i chose Instances and chose the Lab instance already configured.

<img width="1365" height="679" alt="Screenshot 2025-11-25 140930" src="https://github.com/user-attachments/assets/0a483622-2732-4a8d-b645-13e4424bf99e" />

On the left nav menu, i chose Volume under the Elastic Block Store tab. I then created a new volume with the tag My Volume.

<img width="1365" height="678" alt="Screenshot 2025-11-25 141339" src="https://github.com/user-attachments/assets/7f2af1ed-8fff-448d-bc0c-8beab5ed2d0e" />

<img width="1365" height="677" alt="Screenshot 2025-11-25 141447" src="https://github.com/user-attachments/assets/98209976-5da2-472c-8886-136d7ce644d8" />

I then attached the new volume (My Volume) to the pre-existing Lab EC2 instance.

<img width="1365" height="679" alt="Screenshot 2025-11-25 141731" src="https://github.com/user-attachments/assets/7195b2cb-3463-4aba-b96a-7a99a7b38b0d" />

I then connected into the EC2 instance through EC2 Instance Connect. I checked the available storage before making any changes using the command "df -h". Then I created an ext3 file system, created a new directory and mounted the new volume. Then I rechecked the the storage after all the changes and added a text file with some text and mounted it in the new volume.

<img width="1365" height="677" alt="Screenshot 2025-11-25 142039" src="https://github.com/user-attachments/assets/92fb3b9c-8ba5-418a-ace4-4c845f4d2575" />
<img width="1365" height="672" alt="Screenshot 2025-11-25 142148" src="https://github.com/user-attachments/assets/ef6e3604-07c9-4fc7-995d-9952d6753aee" />

I then created an EBS snapsot for My Volume.
<img width="1365" height="677" alt="Screenshot 2025-11-25 143139" src="https://github.com/user-attachments/assets/7a52a0a9-d7dd-42fd-b463-b2ba7c5fd0e2" />

I then created an EBS volume using the snapshot called "Restored Volume". Restored volume was then attached to the volume to the Instance.
<img width="1365" height="680" alt="Screenshot 2025-11-25 143459" src="https://github.com/user-attachments/assets/fd8a6592-a34e-4303-aba9-739794cbb736" />
<img width="1365" height="684" alt="Screenshot 2025-11-25 143659" src="https://github.com/user-attachments/assets/910bac3b-663f-4036-b9fc-c961a4e2fdcc" />

Lastly, i then mounted the Restored Volume by creating a new directory,mounting the volume and verifying the changes by checking the available that the directory is available. in the EC2 Instance Connect Terminal

<img width="1365" height="680" alt="Screenshot 2025-11-25 143919" src="https://github.com/user-attachments/assets/a28c84c7-ebbb-4f67-8cc5-ba9363f24d9b" />

