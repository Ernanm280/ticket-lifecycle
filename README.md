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

<img width="608" alt="Screenshot 2025-01-23 at 12 59 14 PM" src="https://github.com/user-attachments/assets/83f8ebdb-9ddd-4974-bb61-5c2f4ee22e09" />

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

<img width="687" alt="Screenshot 2025-01-23 at 12 59 51 PM" src="https://github.com/user-attachments/assets/a852b748-90c1-4e34-b160-92d4f08c8f39" />
<img width="671" alt="Screenshot 2025-01-23 at 1 00 15 PM" src="https://github.com/user-attachments/assets/0d9f1fb3-dde0-424d-9a31-05e10ee44599" />
<img width="549" alt="Screenshot 2025-01-23 at 1 00 34 PM" src="https://github.com/user-attachments/assets/cc0c62c9-9643-441d-8783-607d14291194" />
<img width="684" alt="Screenshot 2025-01-23 at 1 00 57 PM" src="https://github.com/user-attachments/assets/10ac4f58-82c4-4d72-adc6-d5193358128f" />
<img width="513" alt="Screenshot 2025-01-23 at 1 01 21 PM" src="https://github.com/user-attachments/assets/8204ce0e-db7e-4b70-a625-01950ef3de5c" />

<h2>Purpose </h2>
This repository serves as a practical guide and example of the lifecycle of a ticket within the osTicket system. By following these steps, users can better understand ticket creation, assignment, and resolution workflows in a help desk environment.
