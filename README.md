<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>

This project stimulates real-world IT support scenarios, providing a step-by-step guide to creating and managing tickets within the osTicket system to demonstrate their lifecycle. Each scenario includes steps for creating tickets, observing their properties, setting their attributes, and working them to completion.

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

**Disable/Delete Maintenance Department so tickets don't end up there**

To do this:
  - Navigated to Admin Panel → Agents → Departments
  - Clicked on **Maintenance** and **delete**

> [!NOTE]
> Prevents tickets from being automatically routed to an unused department, ensuring proper ticket flow and visibility.

<img width="945" height="382" alt="Screenshot 2026-02-27 203904" src="https://github.com/user-attachments/assets/e7c484ea-61ae-4dec-8ec6-268e32d3d2cd" />

<h2>Scenarios</h2>

<h3> Scenario 1: Entire Mobile/Online Banking System is Down</h3>

**As an End-User**
1. Navigated to the End Users osTicket URL: [http://localhost/osTicket](http://localhost/osTicket)
2. Logged in as an end-user
3. Created a new ticket with the following details:
  - **Subject**: Entire Mobile/Online Banking System is down
  - **Details**: (Provide a brief description of the issue)
 
> [!NOTE]
> This stimulates a high-impact outage, affecting multiple users and requiring immediate escalation.
 
<img width="833" height="961" alt="Screenshot 2026-02-27 204852" src="https://github.com/user-attachments/assets/2b46feff-4292-48fb-ac4d-b6d736fef038" />

<br>
<br>

**As a Help Desk Agent (John) - Ticket Triage**
1. Navigated to the Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
2. Logged in as "john"

<img width="461" height="362" alt="Screenshot 2026-02-27 221342" src="https://github.com/user-attachments/assets/ddb6d164-9fb5-4e3a-ae92-274099aee6a3" />

<br>
<br>

3. Locate the newly created ticket and observe its properties:
  - Priority
  - Department
  - SLA
  - Assigned To

Observed that John can only view the ticket and leave an internal note.

<img width="946" height="436" alt="Screenshot 2026-02-27 213429" src="https://github.com/user-attachments/assets/ff1fe950-2759-4482-a9c5-c3369dcfef9c" />

<br>
<br>

**Set the ticket properties as follows**:
  - Priority → Sev-A (1 hour SLA)
  - Department → Online Banking Department

> [!NOTE]
>- Sev-A is used for critical outages impacting business operations
>- Assigning to a department ensures the correct team handles the issue

<img width="640" height="260" alt="Screenshot 2026-02-27 212127" src="https://github.com/user-attachments/assets/36a84d49-3736-4a8e-856e-94215669488e" />
<img width="622" height="218" alt="Screenshot 2026-03-01 181306" src="https://github.com/user-attachments/assets/715bb78b-698c-4ba9-ab10-18d8b3be2d65" />

<br>
<br>

**Access Control Observation** 

**After assigning the ticket to a different department, the original agent may lose access since osTicket uses department-based access control. This means agents can only manage a ticket within their assigned department.** 


**As a Help Desk Agent (Jane) - Resolution**
1. Log in as "jane."
2. Investigate and troubleshoot the issue
3. Provide updates to the user
4. Resolve and close the ticket

**Purpose**: Demonstrates full lifecycle completion, including communication and resolution.

<img width="425" height="335" alt="Screenshot 2026-02-27 221709" src="https://github.com/user-attachments/assets/4c734c5a-8593-4cb9-a99f-eefafb483f32" />

<br>
<br>

**The Ticket was escalated to the SysAdmins team, where the root cause was identified as a configuration issue that caused the online banking system to go down. After restarting the server, the service was successfully restored, allowing the workflow to resume.**
**

<img width="971" height="268" alt="Screenshot 2026-02-27 220141" src="https://github.com/user-attachments/assets/fe362cf6-6018-4559-936b-90f90af81e9c" />

<br>
<br>

**The fix was confirmed with the user, and the ticket was marked as resolved and closed.**

<img width="805" height="324" alt="Screenshot 2026-02-27 220431" src="https://github.com/user-attachments/assets/5ac9b35d-5bfb-4bad-9c7a-06cd372b6143" />

<h3>Scenario 2: Accounting Department Needs Adobe Upgrade, Broken</h3>

**As an End-User**
1. Navigate to the End Users osTicket URL: http://localhost/osTicket
2. Log in as an end-user.
3. Create a new ticket with the following details:
  - Subject: Adobe not opening invoices
  - Details: (Provide a brief description of the issue)

<img width="833" height="968" alt="Screenshot 2026-02-27 223047" src="https://github.com/user-attachments/assets/8cbea6f2-9e21-4b4c-b190-4f4163c254da" />

<br>
<br>

**As a Help Desk Agent (John)**
- Navigate to the Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- Log in as "John."
- Locate the newly created ticket and observe its properties:
  - Priority
  - Department
  - SLA
  - Assigned To
 
<img width="461" height="362" alt="Screenshot 2026-02-27 221342" src="https://github.com/user-attachments/assets/d5f46852-101f-4b55-91cc-8bb76fd37a10" />
<img width="950" height="584" alt="Screenshot 2026-02-27 223255" src="https://github.com/user-attachments/assets/5c1c07ff-278b-416a-aefd-ab80735a1841" />

<br>
<br>

- Set the ticket properties as follows:
  - Priority → Sev-B (4 hours SLA)
  - Department → Support Department

**Adjusted the Service Level Agreement (SLA) to Sev-B based on the ticket's business impact. This ensures the issue is prioritized correctly and handled within defined response and resolution timeframes**

<img width="801" height="398" alt="Screenshot 2026-02-27 223530" src="https://github.com/user-attachments/assets/12c374b0-fff5-4f37-93f5-0956ac357741" />

<br>
<br>

**Acknowledged the user's issue and provided a preliminary assessment. Identified that the problem may be due to an outdated version of Adobe Acrobat and communicated the plan to verify and perform an update. Clear expectations were set to ensure commitment and reliability.**

<img width="955" height="634" alt="Screenshot 2026-02-27 223804" src="https://github.com/user-attachments/assets/237711b3-8864-4e35-86df-9d4e2ab823a1" />

<br>
<br>

**Once the issue is resolved, the helpdesk confirmed that Adobe Acrobat has been succesfully updated and tested. The end user was asked to verify functionality to ensure the issue has been resolved.**

<img width="946" height="619" alt="Screenshot 2026-02-27 223852" src="https://github.com/user-attachments/assets/41f89637-2e96-4acf-b6a0-15d6d5e3609e" />

<br>
<br>

**The ticket is marked as resolved, meaning the ticket is now closed.**

<img width="803" height="316" alt="Screenshot 2026-02-27 224103" src="https://github.com/user-attachments/assets/1c62d1a2-82cd-4718-8bd4-04129c63c12a" />


<h3>Scenario 3: CFO’s Laptop Will No Longer Turn On</h3>

**As an End-User**
1. Navigate to the End Users osTicket URL: http://localhost/osTicket
2. Log in as an end-user
3. Create a new ticket with the following details:
  - **Subject**: CFO’s Laptop Will No Longer Turn On
  - **Details**: (Provide a brief description of the issue)

<img width="803" height="960" alt="Screenshot 2026-03-01 172716" src="https://github.com/user-attachments/assets/19b2d4ab-c6ca-452f-a7c6-8af68fab8c1e" />

<br>
<br>

**As a Help Desk Agent (John)**
1. Navigate to the Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
2. Log in as "John"
3. Locate the newly created ticket and observe its properties:
  - Priority
  - Department
  - SLA
  - Assigned To

 **Set the ticket properties as follows**:
  - **Priority** → Sev-B (or Sev-A depending on urgency)
  - **Department** → Support Department

**Why**:
Although it is a single device, it belongs to a high-level executive, making it business-critical.

<img width="948" height="284" alt="Screenshot 2026-03-01 172814" src="https://github.com/user-attachments/assets/e924a27b-1fb6-47f0-a0e9-9984c6cd0551" />

<br>
<br>

**The Tickets SLA was updated to Sev-B after issuing a temporary replacement device. This outlined a reduced business impact since operations were restored and no active outage remained.**

<img width="909" height="443" alt="Screenshot 2026-03-01 173132" src="https://github.com/user-attachments/assets/2dceaaa1-469b-4cd1-8b72-ab2711716c8c" />

<br>
<br>

**The help desk responds to the issue, showing acknowledgment and communicating urgency, recognizing the importance of the users' access to financial reports. Assured the user that troubleshooting was actively in progress.**

<img width="982" height="431" alt="Screenshot 2026-03-01 173459" src="https://github.com/user-attachments/assets/028292b1-a61d-421c-8338-e0a25562e2c5" />

<br>
<br>

**Performed power troubleshooting and determined the device had a hardware failure. Issued a temporary replacement laptop to restore business operations while the original device was sent for further diagnostics and repair.**

<img width="960" height="781" alt="Screenshot 2026-03-01 175356" src="https://github.com/user-attachments/assets/dc09ccbe-9407-4a50-b033-fe6dce9dcc2b" />

<br>
<br>

**The ticket is prepared for closure after restoring user access and ensuring business continuity.**

<img width="657" height="235" alt="Screenshot 2026-03-01 175625" src="https://github.com/user-attachments/assets/bcb9d58f-58de-4167-b7e1-7e82a5a86d87" />

<h2>Purpose </h2>
This repository shows the lifecycle of a support ticket within the osTicket help desk system, demonstrating how technical issues are managed in a structured IT support environment. The project walks through the full ticket workflow, including ticket creation, categorization, assignment to support agents, communication with users, and final resolution. The osTicket system is intended as a hands-on learning exercise to simulate real-world help desk operations and provide practical insight into how ticket management systems function within IT infrastructure environments.
