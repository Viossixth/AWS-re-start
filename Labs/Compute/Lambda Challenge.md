## Lambda Challenge 

**Challenge** 

Your challenge

* Create a Lambda function to count the number of words in a text file. The general steps are as follows:
* Use the AWS Management Console to develop a Lambda function in Python and create the function's required resources.
* Report the word count in an email by using an SNS topic. Optionally, also send the result in an SMS (text) message.

Format the response message as follows:

The word count in the <textFileName> file is nnn. 
Replace <textFileName> with the name of the file.

Enter the following text as the email subject: Word Count Result

Automatically invoke the function when the text file is uploaded to an S3 bucket.

Test the function by uploading a few sample text files with different word counts to the S3 bucket.

Forward the email that one of your tests produces and a screenshot of your Lambda function to your instructor.

**Step 1:SNS Topic & Subscription**

For step one, I went to Amazon SNS and created a topic called word-count-notifications using the standard setting. I then created a subscription, to send message to my email for any alert. The subscription was confirmed and is active.

<img width="1365" height="647" alt="Screenshot 2025-12-17 084845" src="https://github.com/user-attachments/assets/34bca485-0c48-4f40-8a93-cdecd029c2f6" />
<img width="1365" height="645" alt="Screenshot 2025-12-17 085023" src="https://github.com/user-attachments/assets/18a9fb17-5ad1-4220-933a-41d2da3db68c" />
<img width="1365" height="646" alt="Screenshot 2025-12-17 085100" src="https://github.com/user-attachments/assets/0e242547-bfac-4707-92a7-0e2fa395612b" />
<img width="1365" height="645" alt="Screenshot 2025-12-17 085112" src="https://github.com/user-attachments/assets/c5267001-9953-493e-8650-dfbc21f3ce13" />
<img width="1365" height="647" alt="Screenshot 2025-12-17 085327" src="https://github.com/user-attachments/assets/c5dd879a-23ea-4268-9836-4a53f2eda357" />
<img width="1365" height="646" alt="Screenshot 2025-12-17 085342" src="https://github.com/user-attachments/assets/53902a1b-87c1-4d5f-bdeb-22ed85e7d23c" />
<img width="1365" height="646" alt="Screenshot 2025-12-17 085401" src="https://github.com/user-attachments/assets/64d70ee9-2c16-4f86-a357-0bdc1f4ead69" />


**Step 2: S3 Bucket**

I then proceeded back to AWS Management console and searched for S3. Within S3, I created a new bucket called word-ncount-bucket-chris with the default settings.

<img width="1365" height="643" alt="Screenshot 2025-12-17 085910" src="https://github.com/user-attachments/assets/575bfc6b-9323-4e32-bba0-19c0e7851143" />
<img width="1365" height="647" alt="Screenshot 2025-12-17 090042" src="https://github.com/user-attachments/assets/d74bf73d-f9c8-4f7f-99e7-82cace96e05e" />

**Step 3: Lambda Funciton**

For step 3, I went to Lambda and created a function called WordcountFunction. I used Python 3.12 as the runtime and kept the settings as they were. I then changed the code, from the default one to add a new snippet and deployed it.
I added the arn as an environmental variable and also configuered an S3 trigger. 

<img width="1365" height="645" alt="Screenshot 2025-12-17 091037" src="https://github.com/user-attachments/assets/e7e9f911-5ed7-4aef-af76-2eb35ed51b3d" />
<img width="1365" height="647" alt="Screenshot 2025-12-17 091152" src="https://github.com/user-attachments/assets/c5986ab6-9a20-493a-9a8c-b6dff9ae90f8" />
<img width="1365" height="646" alt="Screenshot 2025-12-17 091216" src="https://github.com/user-attachments/assets/bd1dcf09-0cfc-4c77-8e4f-cf2ea33462ef" />
<img width="1365" height="649" alt="Screenshot 2025-12-17 094819" src="https://github.com/user-attachments/assets/45d9d1e1-7da4-4e9c-85d6-0b5462170842" />
<img width="1365" height="645" alt="Screenshot 2025-12-17 091449" src="https://github.com/user-attachments/assets/515c2ced-2831-49cd-a565-0e66d81356bf" />

**Step 4: Testing**

To test if everything is configured properly, I created a .txt file called Lambda test 1 on my notepad. I saved the file and uploaded it into S3. 
I also created another .txt file called Lambda test 2 and uploaded it into S3.


<img width="1365" height="767" alt="Screenshot 2025-12-17 094644" src="https://github.com/user-attachments/assets/459487c6-d257-44ce-a574-23e66c94c9da" />
<img width="1365" height="767" alt="Screenshot 2025-12-17 092330" src="https://github.com/user-attachments/assets/312ee62a-f920-446e-bd2c-5e77895f5196" />
<img width="1365" height="645" alt="Screenshot 2025-12-17 094402" src="https://github.com/user-attachments/assets/4950f4bd-db26-437b-b6cf-9c125b1ab483" />
<img width="685" height="457" alt="Screenshot 2025-12-17 094423" src="https://github.com/user-attachments/assets/ea5b1e0b-f628-433a-a2b7-c25cbdcb0c2c" />
<img width="669" height="461" alt="Screenshot 2025-12-17 094431" src="https://github.com/user-attachments/assets/48117901-c98b-463e-9c35-123d0cc5d4e9" />

**Summary** 

In this Lambda lab i had to create a function that will count the number of words in a document, that will be uploaded to S3. 
The function will read the file, and send an event trigger to SNS with the output to my email address. This was a challenging lab, with many layers to configure and troubleshoot. The one big issue I had was with the arn, and i had copied it wrong somehow but through looking at Cloudwatch logs and seeing that everythign is working except the arn i quickly fixed it.
This Lab took majority of my day, as i head to read some AWS documentation to learn how to setup the services and writing the code was time consuming and a major hurdle.
