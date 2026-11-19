## CLOUD-DATA-STORAGE-SERVER
## NAME: Stephen raj Y
## REG NO: 212223230217
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



