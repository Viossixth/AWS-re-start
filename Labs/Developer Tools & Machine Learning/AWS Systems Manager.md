## AWS Systems Manager

**Task 1: Generate inventory lists for managed instances**

To complete task 1, I logged into the AWS Management Console and searched for Systems Manager. On the landing page, I clicked on Fleet Manager on the left hand navigation. I clicked Account management and setup inventory.
I configured the association as per details given and the association was created successfully.  I clicked the node-id link and checked the inventory and associations page. There was my association which I had created and a list of inventory.

<img width="1365" height="646" alt="Screenshot 2025-12-13 211310" src="https://github.com/user-attachments/assets/5b294e66-a7bc-4186-89b4-9bea2e30e3bf" />
<img width="1365" height="643" alt="Screenshot 2025-12-13 211415" src="https://github.com/user-attachments/assets/0b207bae-4376-40e8-afb1-3a044ef6d3a1" />
<img width="1365" height="645" alt="Screenshot 2025-12-13 211652" src="https://github.com/user-attachments/assets/1162a44a-cdab-4191-8cbe-e983d34cf858" />

**Task 2: Install a Custom Application using Run Command**

<img width="1572" height="808" alt="image" src="https://github.com/user-attachments/assets/f6542547-d830-4428-ac83-9c2e78ee0c7c" />

On the left-hand navigation I clicked Run Command and filtered the options by owner; owned by me. I clicked the document that appeared. 
I configured a few settings, namely target selection, instances and output options. I clicked Run at the bottom, and after a wait of 2 minutes the overall status changed to success. 
I copied the ServerIP value and pasted it into a new tab, and the Widget Manufacturing Dashboard appeared

<img width="1365" height="644" alt="Screenshot 2025-12-13 212318" src="https://github.com/user-attachments/assets/ffa1652c-afad-4f4e-8c2e-0a1f90c49b71" />
<img width="1365" height="645" alt="Screenshot 2025-12-13 212423" src="https://github.com/user-attachments/assets/b1aa2d29-abba-4609-b55f-7fd22af81339" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 213050" src="https://github.com/user-attachments/assets/719769fd-ad04-4f6e-a104-5be253e6c543" />
<img width="1365" height="644" alt="Screenshot 2025-12-13 213416" src="https://github.com/user-attachments/assets/ed014fcb-dbf8-4162-86c2-4308828861ed" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 213449" src="https://github.com/user-attachments/assets/67fee645-eed6-402e-8c03-87f55cae5707" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 213658" src="https://github.com/user-attachments/assets/36996634-0fca-479e-88b3-113c7ed5b4e5" />

**Task 3: Use Parameter Store to manage application settings**

For task 3, I clicked Parameter store on the left navigation menu, and chose create parameter. I configured the parameter using the given details and received a successful message at the end. 
I went to the Widget Manufacturing dashboard to refresh the tab and a third tab appeared. I deleted the parameter and the third chart disappeared.

<img width="1365" height="648" alt="Screenshot 2025-12-13 215021" src="https://github.com/user-attachments/assets/62d29c9a-1a63-43e2-87f5-d8ce80e58d78" />
<img width="1365" height="645" alt="Screenshot 2025-12-13 215030" src="https://github.com/user-attachments/assets/51cb66c2-6ec9-4ea4-966c-dbff5d72204a" />
<img width="1365" height="647" alt="Screenshot 2025-12-13 215113" src="https://github.com/user-attachments/assets/00331f5e-bd82-4cd5-b3b9-d8d83953ad70" />
<img width="1365" height="648" alt="Screenshot 2025-12-13 215130" src="https://github.com/user-attachments/assets/f7c9d27d-3cc8-4d10-b5f0-d702aabdd943" />

**Task 4: Use Session Manager to access instances**

<img width="1594" height="633" alt="image" src="https://github.com/user-attachments/assets/c1792ecf-a435-43c7-9320-43c86949c752" />

For task 4, I had to connect to a session using Session manager under Node Management. I chose start session and selected the Managed Instance and clicked Start session.
On the new tab I ran the command given and ran two more commands to get the region and list information about EC2 instances.

<img width="1365" height="647" alt="Screenshot 2025-12-13 215838" src="https://github.com/user-attachments/assets/a03bd5b4-b86d-4a36-b1f2-39cb264e6569" />
<img width="1365" height="645" alt="Screenshot 2025-12-13 215848" src="https://github.com/user-attachments/assets/e0de6080-5c7f-4e62-8145-6bc3e40187d9" />

<img width="1365" height="647" alt="Screenshot 2025-12-13 215833" src="https://github.com/user-attachments/assets/017f7b49-fffb-4590-bb58-b85f2f4dfc0c" />

<img width="1365" height="647" alt="Screenshot 2025-12-13 220123" src="https://github.com/user-attachments/assets/4dc284f5-32f5-4bc1-b190-145115fb2007" />



