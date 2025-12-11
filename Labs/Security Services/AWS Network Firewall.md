Malware Protection Using an AWS Network Firewall

Task 1: Confirm Access

In this phase of the lab, i use the TestUrl link which directly connect me to my EC2 instance via AWS Systems Manager. 
Upon connection to the instance, I changed directories using the command "cd ~pwd" and then downloaded the malware using wget. I then confirmed if the malware was downloaded using the "ls" command. I 

<img width="1365" height="647" alt="Screenshot 2025-11-26 201825" src="https://github.com/user-attachments/assets/eb7f06c9-2a87-496b-91e8-3a97989222e2" />

<img width="1365" height="648" alt="Screenshot 2025-11-26 202023" src="https://github.com/user-attachments/assets/7d1aef8a-c9d6-4aef-be92-bb725f8becdb" />

Task 2: Inspect the Network Firewall

In this phase of the lab, I logged into the AWS Management Console and searched for VPC. On the VPC page, I chose Firewalls under Ntework Firewall on the left navigation tab. I chose LabFirewall and edited the Stateless deafault actions to forward to stateful rule groups.

<img width="1365" height="644" alt="Screenshot 2025-11-26 202428" src="https://github.com/user-attachments/assets/6e9398d4-fefe-4c61-8d82-a3e41a4678de" />
<img width="1365" height="647" alt="Screenshot 2025-11-26 202636" src="https://github.com/user-attachments/assets/c8d7ac5e-e5b7-43d3-9f26-dea0e6cd75d6" />
<img width="1365" height="644" alt="Screenshot 2025-11-26 212204" src="https://github.com/user-attachments/assets/85381448-a146-4546-87da-81844702d689" />

Task 3: Create a firewall rule group

Under  Network Firewall on the left navigation pane i chose Network Firewall Rule Group. I then created a new rule group.

<img width="1365" height="647" alt="Screenshot 2025-11-26 212534" src="https://github.com/user-attachments/assets/43be136e-524f-4679-b9c4-1b2f9293af7a" />
<img width="1364" height="645" alt="Screenshot 2025-11-26 212727" src="https://github.com/user-attachments/assets/affbe3ca-bc94-42fa-89a5-44d07f3576dd" />

Task 4: Attach a rule group to the network firewall

For task 4, I chose Firewalls under Network Firewall. I chose the created firewall " LabFirewall" and selected the LabFirewallPolicy under Associated firewall policy. I added a stateful rule group where it says Add unmanaged stateful rule groups under Stateful rule groups.

<img width="1365" height="643" alt="Screenshot 2025-11-26 213044" src="https://github.com/user-attachments/assets/60e899c2-561b-4329-822e-521429a9bc8c" />
<img width="1365" height="645" alt="Screenshot 2025-11-26 213054" src="https://github.com/user-attachments/assets/66586176-1a0a-4518-81ff-039fea021de9" />

<img width="1365" height="646" alt="Screenshot 2025-11-26 213218" src="https://github.com/user-attachments/assets/459ab3e0-2b13-450d-897b-01c064387fe1" />
<img width="1365" height="645" alt="Screenshot 2025-11-26 213241" src="https://github.com/user-attachments/assets/97f33a5f-bbcc-488b-8aee-ad7d28719d48" />

Task 5: Validation

I went to EC2 through the AWS Management Console, and connected to the TestInstance through the session manager. Once connected i changed the directories by using the " cd ~pwd" command, i tried to get the malicious file using the "wget" command and received a waiting response. I tried it again with another file using "wget" but got the same wait response. I then deleted the two malicious files and confirmed using the "ls" command.

<img width="1365" height="643" alt="Screenshot 2025-11-26 213617" src="https://github.com/user-attachments/assets/70e97fed-c3d7-45a1-8ed7-73277cd4057b" />
<img width="1365" height="645" alt="Screenshot 2025-11-26 213622" src="https://github.com/user-attachments/assets/f3c819f8-6beb-427d-ad06-77e51cb7c85f" />
<img width="1365" height="647" alt="Screenshot 2025-11-26 213753" src="https://github.com/user-attachments/assets/277caab9-0f92-437f-86d6-0d6c5daa9b26" />



