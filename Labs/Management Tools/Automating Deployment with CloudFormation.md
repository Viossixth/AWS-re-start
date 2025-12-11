## Automating Deployments with AWS CloudFormation

<img width="2391" height="1142" alt="image" src="https://github.com/user-attachments/assets/8d19535a-1d2a-4e8b-8684-292ccc85b4a9" />

**Overview**

To complete this lab, I had to crreate a CloudFormation stack, add an Amazon S3 Bucket to the stack via an update and update the template again to add an EC2 Instance. To complete the Lab i had to delete the configured stack.

**Task 1 : Configure a CloudFromation stack**

<img width="1365" height="643" alt="Screenshot 2025-12-11 170907" src="https://github.com/user-attachments/assets/43027407-1940-4f78-b6ed-dc7f8f7cb8fc" />
<img width="1365" height="644" alt="Screenshot 2025-12-11 170949" src="https://github.com/user-attachments/assets/3dd9e19a-d71d-486f-938e-1a778622003e" />
<img width="1365" height="644" alt="Screenshot 2025-12-11 171240" src="https://github.com/user-attachments/assets/2091d69d-a04c-4051-99b0-d28d5a4467da" />
<img width="1365" height="649" alt="Screenshot 2025-12-11 171415" src="https://github.com/user-attachments/assets/74f022b2-11f3-4816-9ba3-db4ae362c578" />
<img width="1365" height="645" alt="Screenshot 2025-12-11 171457" src="https://github.com/user-attachments/assets/a0daad0c-3274-491d-8ea0-85e8eadee765" />


In this phase I had to configure a new CloudFormation Stack using a YAML Template already written with the resources to be added. I configured the stack and created it.

**Task 2: Update Template to add an S3 Bucket**

In this phase, I had to update the YAML Template to add an S3 Bucket to the resources, this step needed me to look at the documentation and after change the template.
The changes were two lines and the update was successful.

<img width="1365" height="643" alt="Screenshot 2025-12-11 172715" src="https://github.com/user-attachments/assets/c9c99840-8eec-4bb9-9f23-ddc47035701d" />
<img width="1365" height="645" alt="Screenshot 2025-12-11 172832" src="https://github.com/user-attachments/assets/3dc02912-997b-4996-b0bf-48e8b07d2bf3" />
<img width="1365" height="642" alt="Screenshot 2025-12-11 172845" src="https://github.com/user-attachments/assets/bc4f77d9-8e24-4066-8a57-7276e623e7b7" />
<img width="1365" height="648" alt="Screenshot 2025-12-11 172956" src="https://github.com/user-attachments/assets/c47f9523-5d0a-458a-9094-3ade98dc2142" />
<img width="1365" height="643" alt="Screenshot 2025-12-11 173016" src="https://github.com/user-attachments/assets/d1fecafc-e807-420b-a5c3-be11f32810fa" />

**Task 3: Update Template to add an EC2 Instance**

In this phase, I had to update the Parameters section of the Template and after adding the changes i also had to update the resources section. 
I had to ensure that the resources and Parameters referenced each other perfectly, otherwise the Template would have issues when updating and a rollback would be needed.
I also went to EC2 to check the dashboard to confirm if the Instance was created.

<img width="1365" height="767" alt="Screenshot 2025-12-11 173117" src="https://github.com/user-attachments/assets/e0cbe334-2055-4565-bb24-e161e832b147" />
<img width="1365" height="767" alt="Screenshot 2025-12-11 182413" src="https://github.com/user-attachments/assets/0094be01-ede1-4bb9-a8c3-285ddfbfb58e" />
<img width="1365" height="644" alt="Screenshot 2025-12-11 174844" src="https://github.com/user-attachments/assets/86fceed1-4932-4b02-9f0a-d15d48ca405a" />
<img width="1365" height="646" alt="Screenshot 2025-12-11 174908" src="https://github.com/user-attachments/assets/7330197a-61ab-4007-af62-3b94a6080f6a" />

<img width="1365" height="645" alt="Screenshot 2025-12-11 174924" src="https://github.com/user-attachments/assets/4f6c32bf-30ba-41cf-9f6a-83807f6c7f1b" />

<img width="1365" height="643" alt="Screenshot 2025-12-11 180534" src="https://github.com/user-attachments/assets/9730fa05-b7fd-4498-bdd4-bbe099497793" />
<img width="1365" height="645" alt="Screenshot 2025-12-11 180615" src="https://github.com/user-attachments/assets/d856bef3-7cf9-4035-a116-e05049294eec" />


**Task 4: Delete CloudFront Stack**

In this last phase I had to delete the stack that i created with all resources. I deleted the stack and confirmed that no one stack remained on CloudFront.

<img width="1365" height="645" alt="Screenshot 2025-12-11 180632" src="https://github.com/user-attachments/assets/cbb4eb92-d925-401e-ad13-35cd2988062f" />
<img width="1365" height="646" alt="Screenshot 2025-12-11 180647" src="https://github.com/user-attachments/assets/9c1f7d9b-4d6d-4d2f-9777-d6b1937b26d7" />
<img width="1365" height="648" alt="Screenshot 2025-12-11 180750" src="https://github.com/user-attachments/assets/8a2c0f7c-a32c-416d-a4ab-c857fd3639a9" />
