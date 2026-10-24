Part A: Dotnet (35 Marks)
Employee Management System

Problem Statement

Develop an ASP.NET Core MVC application using Entity Framework Core to manage employee information.

Employee Details

Create an Employee model with the following fields:

Id

Name

Department

Salary


Requirements

1. Create Database

Use:

· Entity Framework Core

· SQL Server

· Code First Approach

Perform:

Shell

Add-Migration InitialCreate

Update-Database


---

2. Implement CRUD Operations

Employee should support:

✅ Create Employee

✅ View Employee List

✅ Edit Employee

✅ Delete Employee

---


Files They Should Create

Plain Text

Models

└── Employee.cs


Data

└── AppDbContext.cs


Controllers

└── EmployeeController.cs


Views

└── Employee

├── Index.cshtml

├── Create.cshtml

├── Edit.cshtml

└── Delete.cshtml



Build the and publish it
<img width="1280" height="683" alt="image" src="https://github.com/user-attachments/assets/67f09cd4-8517-4f73-86db-8e74adb35bf8" />
<img width="1280" height="686" alt="image" src="https://github.com/user-attachments/assets/edf2ef4c-7709-4f12-a200-947d6615e147" />

======================================================================================
Part B: Windows administration:

Windows Server 2022 Practical Assessment

---

Scenario

You have been assigned as a Junior Windows Server Administrator. A new file server has been deployed and needs initial configuration, user management, storage configuration, permissions assignment, and troubleshooting.

Complete all tasks using GUI tools only (Server Manager, Computer Management, Disk Management, Task Manager, Resource Monitor, Services Console).

PartB
Task 1:
Task 1: Server Information and Configuration (5 Marks)

Requirements

1. Identify the Windows Server edition installed.

2. Identify:

o Computer Name

o IP Address

o RAM

o CPU Information

3. Rename the server to:

<YOUR_NAME>-SRV01

Evaluation

<img width="490" height="523" alt="image" src="https://github.com/user-attachments/assets/8f073012-b54d-480c-acb9-c1ac25cc8ea3" />

<img width="1280" height="520" alt="image" src="https://github.com/user-attachments/assets/ad7a57ed-3009-437c-bfb3-5caea7c5abd3" />
<img width="645" height="577" alt="image" src="https://github.com/user-attachments/assets/dcbec0d8-ab21-4f54-9fae-9e6dcea8385f" />

==========================================================================================

PartB
Task 2:
Task 2: Roles and Server Manager (5 Marks)

Requirements

Using Server Manager:

1. Identify currently installed roles.

2. Install the following role:

o File Server
<img width="1280" height="675" alt="image" src="https://github.com/user-attachments/assets/39423d90-215f-4b41-8f4c-4668ce94e169" />

==========================================================================================

PartB
Task 3:
Task 3: User and Group Administration (10 Marks)

Requirements

Create the following local users:

Plain Text

<YOUR_NAME>-finance01

<YOUR_NAME>-finance02


Create local groups:

FinanceUsers

FileAdmins

Perform:

1. Add both users to FinanceUsers.

2. Add finance01 to FileAdmins.

3. Set password:

4. P@ssw0rd123

5. Configure:

o Password never expires

o User must change password at next logon disabled

Evaluation
Users
<img width="986" height="458" alt="image" src="https://github.com/user-attachments/assets/443249bd-2126-4a71-8ac4-628e2fcb6bd6" />

Groups
<img width="973" height="455" alt="image" src="https://github.com/user-attachments/assets/144fa71e-3aa0-4cbb-adf8-ebc947a49710" />

Users Assign to Groups
<img width="399" height="453" alt="image" src="https://github.com/user-attachments/assets/8dc1a145-0c4b-4adc-9e12-a3d7f283299a" />
<img width="402" height="455" alt="image" src="https://github.com/user-attachments/assets/ee1ac959-8364-466d-80e1-a753689aaa89" />


============================================================================================
PartB
Task 4:
Task 4: File System and NTFS Permissions (10 Marks)

Requirements

Create folder structure:

D:\CompanyData

D:\CompanyData\<YOUR_NAME>-Finance

D:\CompanyData\<YOUR_NAME>-HR

Configure permissions:

<YOUR_NAME>-Finance Folder

Remove Users group.

Grant:

FinanceUsers = Modify

Administrators = Full Control

Verify resulting permissions.
<img width="764" height="520" alt="image" src="https://github.com/user-attachments/assets/ff37baec-e960-45fd-9086-df9ef38dd5d3" />

==============================================================

PartB
Task 5:
Task 5: Shared Folder Configuration (10 Marks)

Requirements

Share:

D:\CompanyData\<YOUR_NAME>-Finance


Share name:

FinanceShare

Configure:

Group Share Permission
<img width="398" height="480" alt="image" src="https://github.com/user-attachments/assets/f5014560-aa03-4fe5-b549-8ef4225c16f7" />

===================================
PartB
Task 7:
Task 7: Storage Management (10 Marks)

Requirements

A new disk is attached.

Perform:

1. Bring disk Online.

2. Initialize as GPT.

3. Create Simple Volume.

4. Format NTFS.

5. Assign drive letter:

<YOUR_NAME>-F:

6. Create volume label:

Plain Text

DATA
<img width="748" height="589" alt="image" src="https://github.com/user-attachments/assets/7718b05b-d748-487b-aa0c-ce1d488af4c3" />
<img width="365" height="520" alt="image" src="https://github.com/user-attachments/assets/a3c27f5a-e4a2-4db9-863c-573d20c86961" />

===================================

PartB
Task 9:
Task 9: Process Monitoring and Troubleshooting (5 Marks)

Requirements

Using Task Manager and Resource Monitor:

1. Identify process consuming highest CPU.

2. Identify process consuming highest memory.

3. Sort processes by CPU utilization.

4. Record:

o Process Name

o PID

o CPU %

o Memory Usage

1. Highest cpu utilization
<img width="1278" height="613" alt="image" src="https://github.com/user-attachments/assets/2081e662-2a55-4815-a2cb-79684f73075f" />

2. Highest memory utilization
<img width="1117" height="559" alt="image" src="https://github.com/user-attachments/assets/8b3b11dd-46e2-43a2-9c70-08e0fab0eed6" />

3. Sort processes by CPU utilization.
<img width="1267" height="641" alt="image" src="https://github.com/user-attachments/assets/02f09644-5693-4a57-8c8e-8f81b6dd272f" />

4. Record:
o Process Name
o PID
o CPU %
o Memory Usage
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/58a5aad3-5767-41f8-9c6e-623e7b272185" />

=========================================

PartB
Task 10:
Task 10: Services Administration and Recovery (5 Marks)

Requirements

Using Services Console:

1. Locate Print Spooler service.

2. Stop service.

3. Start service.

4. Configure:

5. First Failure = Restart Service

6. Identify one dependent service.

Stopped service 
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/923b72e3-5ac6-4f5c-af48-b2e5b11f4828" />

Running Service 
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/9781d7f8-edec-4bfb-8464-731c6b1e2900" />

Dependent Service
<img width="417" height="471" alt="image" src="https://github.com/user-attachments/assets/d1daba2a-0ec8-44f4-9fce-4b3bef3b5aef" />
