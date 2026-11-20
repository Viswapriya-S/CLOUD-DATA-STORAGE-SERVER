## CLOUD-DATA-STORAGE-SERVER
## NAME: Viswapriya S
## REG NO: 212225230311
## Aim:
To create and configure an Amazon Relational Database Service (Amazon RDS) instance as a cloud data storage server, configure the required security settings, connect it to a web application, and perform database operations using the application.

## Algorithm / Steps
1.Create a Security Group for the RDS database.
2.Add an inbound rule to allow MySQL (Port 3306) access from the Web Security Group.
3.Create a DB Subnet Group using two Availability Zones.
4.Launch an Amazon RDS MySQL database instance.
5.Configure the database with the required identifier, username, password, storage, and instance class.
6.Associate the database with the created Security Group and Subnet Group.
7.Wait until the database status becomes Available.
8.Copy the RDS endpoint.
9.Open the web application using the provided Web Server IP address.
10.Enter the RDS endpoint, database name, username, and password.
11.Connect the application to the database.
12.Verify the connection by adding, editing, and deleting records in the Address Book application.
## Program
## Security Group Configuration
  Security Group Name: DB Security Group
  Inbound Rule: MySQL/Aurora (3306)
  Source: Web Security Group
## DB Subnet Group
  Name: DB-Subnet-Group
  VPC: Lab VPC
## Amazon RDS Configuration
  Engine: MySQL
  Template: Dev/Test
  Availability: Multi-AZ
  DB Instance Identifier: lab-db
  Username: main
  Password: lab-password
  Instance Class: db.t3.micro
  Storage: 20 GB (General Purpose SSD)
## Connect the Application
  Endpoint : <RDS Endpoint>
  Database : lab
  Username : main
  Password : lab-password
After submitting the above details, perform Add, Edit, and Delete operations on the Address Book application.

## Output:

<img width="1920" height="1080" alt="Screenshot (83)" src="https://github.com/user-attachments/assets/b9f344d0-274d-413e-941d-917d8e14d6a0" />0
<img width="1920" height="1080" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/c858d84b-cc90-40d8-bbea-faf121e7629f" />
<img width="1920" height="1080" alt="Screenshot (85)" src="https://github.com/user-attachments/assets/f9aba9b9-eef8-4a18-8d4b-9faf1cc4dd31" />
<img width="1920" height="1080" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/24cf9982-b22b-4863-94c6-814909f7ffc9" />
<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/85de38ae-0914-4617-9989-c4c04820304d" />
<img width="1920" height="1080" alt="Screenshot (88)" src="https://github.com/user-attachments/assets/2c13c641-543e-4dfc-abdb-038fb6eb6898" />
<img width="1920" height="1080" alt="Screenshot (89)" src="https://github.com/user-attachments/assets/4f096492-f93e-446b-8353-5eb2c0932fb0" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/733f3eaf-7d41-47f4-94d9-7bbe1e366133" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e8477e4d-f4d1-423b-b513-242c7bb51802" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c85cf284-8246-42ff-925c-d6135bdaa55a" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fae81084-0b3f-4490-8c4f-c6ab63ea5eac" />

## Result:
Thus, an Amazon RDS database instance was successfully created and configured as a cloud data storage server. The database was securely connected to a web application, and data operations such as inserting, updating, and deleting records were successfully performed through the application.

