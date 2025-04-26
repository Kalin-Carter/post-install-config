<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Microsoft Azure
- Windows Virtual Machine
- Remote Desktop
- osTicket
- Internet Information Services (IIS)

<h2>Configuration Steps</h2>

<p>
  
![4DCE9871-1483-4A2E-AE1F-0DA3F00D7E2F_1_105_c](https://github.com/user-attachments/assets/bcc75a9b-e1ca-49c9-830d-9b6bd00e766c)

![02DDC4A9-C0CC-4D4D-A5F7-680280435934_1_105_c](https://github.com/user-attachments/assets/8b484039-47f9-4638-9356-c3bccb91945d)

</p>
<p>
Acknowledge Agent Panel vs Admin Panel

Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
Supreme Admin
Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins

</p>
<br />

<p>
  
![F1C03E29-111A-438F-A7F9-7EA1A1A61D03_1_105_c](https://github.com/user-attachments/assets/5d168720-1d64-4730-bc79-d9a1625cd97f)
  
</p>
<p>

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking
Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

</p>
<br />

<p>
  
![8B94C761-E629-414B-A9A3-DF3EEBEA5378_1_105_c](https://github.com/user-attachments/assets/d23eeb8a-d4e6-4cd4-8c7e-d2fcb1d22ef6)

</p>
<p>
Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)
Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

![7BC445FC-FA15-4146-98F5-6DADE939BCA4_1_105_c](https://github.com/user-attachments/assets/25b2fc64-9aee-442d-bc70-752cf2f2ee7f)


Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)
Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other


