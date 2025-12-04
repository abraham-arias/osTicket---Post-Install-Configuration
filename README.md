<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket — Post-Installation Configuration  
This guide outlines the **post-installation setup and configuration** for the open-source help desk ticketing system **osTicket**.  
These steps simulate real-world help desk administration tasks typically handled by IT Support, Help Desk, and System Administrator teams.

---

## 🧰 Environments & Technologies Used
- Microsoft Azure (Virtual Machines / Compute)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

---

## 💻 Operating System Used
- **Windows 10 (21H2)**

---

# 🧪 Post-Install Configuration Steps

## 🔹 **Step 1 — Configure Roles**
Create a high-level administrative role with full permissions.

**Admin Panel → Agents → Roles → Add New Role**

- Name: **Supreme Admin**
- Under *Permissions*, enable **every** permission category  
  (This grants unrestricted access for administrative tasks.)

<br/>

<img src="https://i.imgur.com/AxZLAMB.png"/>

---

## 🔹 **Step 2 — Configure Departments**
Departments help organize agent responsibilities within the help desk.

**Admin Panel → Agents → Departments → Add New Department**

- Name: **System Administrators**
- Leave default settings and click **Create Department**

<br/>

<img src="https://i.imgur.com/DL5ebHM.png"/>

---

## 🔹 **Step 3 — Configure Teams**
Teams allow collaboration between agents across departments.

**Admin Panel → Agents → Teams → Add New Team**

- Team Name: **Level II Support**
- Under **Members**, add yourself as a team member

<br/>

<img src="https://i.imgur.com/qOP1yxp.png"/>

---

## 🔹 **Step 4 — Allow Users to Create Tickets Without Accounts**
Enable the option for anyone to submit tickets, even without registering.

**Admin Panel → Settings → Users → Settings**

Uncheck:

- **Require registration and login to create tickets**

<br/>

<img src="https://i.imgur.com/uhD9R6y.png"/>

---

## 🔹 **Step 5 — Configure Agents**
Agents are the help desk professionals who work and resolve tickets.

**Admin Panel → Agents → Add New Agent**

### Create Agent #1 — Jose Perez
- **Name:** Jose Perez  
- **Email:** jose.perez@osticket.com  
- **Username:** jose.perez  
- Set a password manually  
- Uncheck: “Send password reset email”  
- Uncheck: “Require password change at next login”

### Assign Access & Team Membership
- **Department:** System Admin → Senior Admin  
- **Team:** Level II Support  
- Click **Create**

### Create Agent #2 — Richard Mills
- **Name:** Richard Mills  
- Assign:
  - **Department:** Support (View Only)  
  - **Team:** None (or based on your design)

<br/>

<img src="https://i.imgur.com/QexHP1d.png"/>

---

## 🔹 **Step 6 — Configure Users**
Users are the individuals who submit tickets.

Switch to the **Agent Panel**:

**Users → Create New User**

### Add the following users:
1. **Maria Larson**  
   - maria.larson@osticket.com  

2. **John Wick**  
   - john.wick@osticket.com  

<br/>

<img src="https://i.imgur.com/nqd72sj.png"/>

---

## 🔹 **Step 7 — Configure SLA Plans**
Service Level Agreements define how quickly tickets must be resolved.

**Admin Panel → Manage → SLA → Add New SLA Plan**

Create these SLA plans:

| SLA Name | Grace Period | Schedule |
|---------|--------------|----------|
| **SEV A** | 1 hour | 24/7 |
| **SEV B** | 4 hours | 24/7 |
| **SEV C** | 8 hours | Monday–Friday |

<br/>

<img src="https://i.imgur.com/Y0XNLPD.png"/>

---

## 🔹 **Step 8 — Configure Help Topics**
Help topics streamline the ticket submission and routing process.

**Admin Panel → Manage → Help Topics → Add New Help Topic**

Create the following help topics:

- Business Critical Outage  
- Personal Computer Issues  
- Equipment Request  
- Password Reset  

<br/>

<img src="https://i.imgur.com/aX2RVgn.png"/>

---

# 🎉 osTicket Post-Install Configuration Complete!
You now have:

- Defined **roles**, **departments**, and **teams**  
- Added **agents** and **users**  
- Configured **SLAs** and **help topics**  
- Enabled user-friendly ticket submission  

This reflects real-world responsibilities of IT Support and Help Desk Administrators.

---

# 🧠 Skills Demonstrated
- Help desk administration  
- Role-based access control (RBAC)  
- Ticket workflow configuration  
- User and agent management  
- SLA planning  
- System configuration in a cloud-hosted environment  

---

# 📄 Summary
This project showcases your ability to perform foundational help desk administration tasks—essential for roles like:

- IT Support Specialist  
- Help Desk Technician  
- Desktop Support Technician  
- Junior System Administrator  

