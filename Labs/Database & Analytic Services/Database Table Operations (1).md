###Table Operations in a Database 

The main aim of this lab is to use common database table operations such as Create ,Show , Alter and Drop. These are the main operations used on a database daily.

<img width="864" height="534" alt="Screenshot 2025-11-24 144521" src="https://github.com/user-attachments/assets/7e2c8856-28b4-4c06-a750-eab7e2fcfdd7" />

To start this lab, i had to login into the AWS Management Console and search for EC2. I clicked EC2 and went to the instances, and selected command host (the instance available).I used Sesion Manager to connect to the EC2 instance using the connect button.

<img width="1365" height="643" alt="Screenshot 2025-11-24 211324" src="https://github.com/user-attachments/assets/c51c16ba-4830-4a38-ae54-6b38a8171e5d" />
<img width="1365" height="645" alt="Screenshot 2025-11-24 211349" src="https://github.com/user-attachments/assets/c7ce9070-6df1-47f3-b7bf-e88c1db82753" />

Once I connected to the EC2 instance, i had to use the "sudo su" command to change the directory into the directory of the EC2 user. Sudo su ,allows you to make changes as the root user with elevated permission above other users. Sudo stands for Super User DO and SU stands for SuperUser. After changind directories, i had to log into Mysql using the root user credentials and password.

<img width="1365" height="647" alt="Screenshot 2025-11-24 211451" src="https://github.com/user-attachments/assets/564456cf-c77f-427a-82c9-941b0b86167f" />

The first operations to be used is Show and I used it to view all the databases present upon loging in.

<img width="1365" height="646" alt="Screenshot 2025-11-24 211638" src="https://github.com/user-attachments/assets/e930da55-ddeb-44c2-95ff-a17a9368261d" />

The second operation is create, used to create a new database or table. In this instance I created a new database called world and a new table called country within the world database. After creating the table, I inserted columns and rows into the table specifying the primary keys, not null (where needed) and the type of data to be inserted ( CHAR or FLOAT)

The third operation is alter used to change various information. In this instance it was used to make a change in the table country, renaming the Conitinent to continent. It is helpful in instances where typos are discovered and need to be changed or in the case of columns are re-purposed for new information.

<img width="1365" height="647" alt="Screenshot 2025-11-24 220457" src="https://github.com/user-attachments/assets/08357d7f-4856-4ed1-a1bf-22f3fbf3992b" />

The last operation is drop used to permanently delete tables or an entire database. Care must be taken to use the Drop operations when confirmed to avoid mistakes.

<img width="1365" height="648" alt="Screenshot 2025-11-24 220507" src="https://github.com/user-attachments/assets/37353220-3f8f-480d-83a9-1b300a1bc334" />
