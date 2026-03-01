<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>

This document provides a step-by-step guide to creating and managing tickets within the osTicket system to demonstrate their lifecycle. Each scenario includes steps for creating tickets, observing their properties, setting their attributes, and working them to completion.

Admin/Analyst Login Page: [Admin Login](http://localhost/osTicket/scp/login.php)

End Users osTicket URL: [End Users Ticketing Page](http://localhost/osTicket)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Before you Start</h2>

Disable/Delete Maintenance Department so tickets don't end up there.
To do this:
  - Navigate to Admin Panel -> Agents -> Departments.
  - Click on Maintenance and delete
<img width="945" height="382" alt="Screenshot 2026-02-27 203904" src="https://github.com/user-attachments/assets/e7c484ea-61ae-4dec-8ec6-268e32d3d2cd" />

<h2>Scenarios</h2>

<h3> Scenario 1: Entire Mobile/Online Banking System is Down</h3>

**As an End-User**
- Navigate to the End Users osTicket URL: [http://localhost/osTicket](http://localhost/osTicket)
- Log in as an end-user.
- Create a new ticket with the following details:
  - Subject: Entire Mobile/Online Banking System is Down
  - Details: Provide a brief description of the issue.
 
<img width="833" height="961" alt="Screenshot 2026-02-27 204852" src="https://github.com/user-attachments/assets/2b46feff-4292-48fb-ac4d-b6d736fef038" />

**As a Help Desk Agent (John)**
- Navigate to the Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- Log in as "john."
- Locate the newly created ticket and observe its properties:
  - Priority
  - Department
  - SLA
  - Assigned To
- Set the ticket properties as follows:
  - Priority: Sev-A (1 hour, 24/7)
  - Department: Online Banking Department
- Attempt to observe the ticket again as "john" and note whether you can view or change it.

<img width="461" height="362" alt="Screenshot 2026-02-27 221342" src="https://github.com/user-attachments/assets/ddb6d164-9fb5-4e3a-ae92-274099aee6a3" />
<img width="622" height="218" alt="Screenshot 2026-03-01 181306" src="https://github.com/user-attachments/assets/715bb78b-698c-4ba9-ab10-18d8b3be2d65" />
<img width="640" height="260" alt="Screenshot 2026-02-27 212127" src="https://github.com/user-attachments/assets/36a84d49-3736-4a8e-856e-94215669488e" />
<img width="639" height="253" alt="Screenshot 2026-02-27 212235" src="https://github.com/user-attachments/assets/26ff2cc2-f00d-48b9-a878-0dbbbf544c10" />
<img width="946" height="436" alt="Screenshot 2026-02-27 213429" src="https://github.com/user-attachments/assets/ff1fe950-2759-4482-a9c5-c3369dcfef9c" />

**As a Help Desk Agent (Jane)**
- Log in as "jane."
- Work the ticket to completion.

<img width="425" height="335" alt="Screenshot 2026-02-27 221709" src="https://github.com/user-attachments/assets/4c734c5a-8593-4cb9-a99f-eefafb483f32" />
<img width="971" height="268" alt="Screenshot 2026-02-27 220141" src="https://github.com/user-attachments/assets/fe362cf6-6018-4559-936b-90f90af81e9c" />
<img width="805" height="324" alt="Screenshot 2026-02-27 220431" src="https://github.com/user-attachments/assets/5ac9b35d-5bfb-4bad-9c7a-06cd372b6143" />


<h3>Scenario 2: Accounting Department Needs Adobe Upgrade, Broken</h3>

**As an End-User**
- Navigate to the End Users osTicket URL: http://localhost/osTicket
- Log in as an end-user.
- Create a new ticket with the following details:
  - Subject: Accounting Department Needs Adobe Upgrade, Broken
  - Details: Provide a brief description of the issue.

<img width="833" height="968" alt="Screenshot 2026-02-27 223047" src="https://github.com/user-attachments/assets/8cbea6f2-9e21-4b4c-b190-4f4163c254da" />

**As a Help Desk Agent (John)**
- Navigate to the Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- Log in as "John."
- Locate the newly created ticket and observe its properties:
  - Priority
  - Department
  - SLA
  - Assigned To
- Set the ticket properties as follows:
  - Priority: Sev-B (4 hours, 24/7)
  - Department: Support
- Work the ticket to completion.

<img width="461" height="362" alt="Screenshot 2026-02-27 221342" src="https://github.com/user-attachments/assets/d5f46852-101f-4b55-91cc-8bb76fd37a10" />
<img width="950" height="584" alt="Screenshot 2026-02-27 223255" src="https://github.com/user-attachments/assets/5c1c07ff-278b-416a-aefd-ab80735a1841" />
<img width="801" height="398" alt="Screenshot 2026-02-27 223530" src="https://github.com/user-attachments/assets/12c374b0-fff5-4f37-93f5-0956ac357741" />
<img width="955" height="634" alt="Screenshot 2026-02-27 223804" src="https://github.com/user-attachments/assets/237711b3-8864-4e35-86df-9d4e2ab823a1" />
<img width="946" height="619" alt="Screenshot 2026-02-27 223852" src="https://github.com/user-attachments/assets/41f89637-2e96-4acf-b6a0-15d6d5e3609e" />
<img width="803" height="316" alt="Screenshot 2026-02-27 224103" src="https://github.com/user-attachments/assets/1c62d1a2-82cd-4718-8bd4-04129c63c12a" />


<h3>Scenario 3: CFO’s Laptop Will No Longer Turn On</h3>

**As an End-User**
- Navigate to the End Users osTicket URL: http://localhost/osTicket
- Log in as an end-user.
- Create a new ticket with the following details:
  - Subject: CFO’s Laptop Will No Longer Turn On
  - Details: Provide a brief description of the issue.

<img width="803" height="960" alt="Screenshot 2026-03-01 172716" src="https://github.com/user-attachments/assets/19b2d4ab-c6ca-452f-a7c6-8af68fab8c1e" />

**As a Help Desk Agent (John)**
- Navigate to the Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- Log in as "John."
- Locate the newly created ticket and observe its properties:
  - Priority
  - Department
  - SLA
  - Assigned To
- Set the ticket properties as follows:
  - Priority: Sev-B (4 hours, 24/7)
  - Department: Support
- Work the ticket to completion.

<img width="948" height="284" alt="Screenshot 2026-03-01 172814" src="https://github.com/user-attachments/assets/e924a27b-1fb6-47f0-a0e9-9984c6cd0551" />
<img width="909" height="443" alt="Screenshot 2026-03-01 173132" src="https://github.com/user-attachments/assets/2dceaaa1-469b-4cd1-8b72-ab2711716c8c" />
<img width="982" height="431" alt="Screenshot 2026-03-01 173459" src="https://github.com/user-attachments/assets/028292b1-a61d-421c-8338-e0a25562e2c5" />
<img width="960" height="781" alt="Screenshot 2026-03-01 175356" src="https://github.com/user-attachments/assets/dc09ccbe-9407-4a50-b033-fe6dce9dcc2b" />
<img width="657" height="235" alt="Screenshot 2026-03-01 175625" src="https://github.com/user-attachments/assets/bcb9d58f-58de-4167-b7e1-7e82a5a86d87" />

<h2>Purpose </h2>
This repository serves as a practical guide and example of the lifecycle of a ticket within the osTicket system. By following these steps, users can better understand ticket creation, assignment, and resolution workflows in a help desk environment.
