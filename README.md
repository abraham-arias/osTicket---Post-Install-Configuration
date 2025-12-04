<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket — Post-Installation Configuration  
This phase focuses on configuring the help desk environment after installation.  
These post-install tasks simulate what a real **Help Desk Administrator** or **System Administrator** does to prepare a production-ready support system.

---

# 📘 Project Overview
In this lab, I configured:

- Roles & permissions  
- Departments  
- Support teams  
- Agents & end users  
- SLAs (Service Level Agreements)  
- Help topics  

Each configuration element mirrors a real-world IT support workflow used to organize ticket routing, role-based access control, and service prioritization.

---

# 🧰 Environments & Technologies Used
- Microsoft Azure VM
- osTicket Admin Panel
- Windows 10 (21H2)
- IIS / PHP

---

# 🛠️ Configuration Steps

## 🔹 Step 1 — Create Administrative Roles
**Admin Panel → Agents → Roles → Add New Role**

Create **Supreme Admin** role → grant *all* permissions.

<br/>

<img src="https://i.imgur.com/AxZLAMB.png"/>

This role represents unrestricted administrative access for system configuration.

---

## 🔹 Step 2 — Create Departments
Departments define areas of responsibility.

**Admin Panel → Agents → Departments → Add New Department**

- Name: **System Administrators**
- Keep default settings

<br/>

<img src="https://i.imgur.com/DL5ebHM.png"/>

---

## 🔹 Step 3 — Configure Teams
Teams allow agents to collaborate across departments.

**Admin Panel → Agents → Teams → Add New Team**

- Team Name: **Level II Support**
- Add yourself under **Members**

<br/>

<img src="https://i.imgur.com/qOP1yxp.png"/>

---

## 🔹 Step 4 — Allow Public Ticket Creation
Enable users to create tickets without logging in.

**Admin Panel → Settings → Users → Settings**

Uncheck:

- **Require registration and login to create tickets**

<br/>

<img src="https://i.imgur.com/uhD9R6y.png"/>

---

## 🔹 Step 5 — Create Agents
Agents resolve tickets and require appropriate permissions.

**Admin Panel → Agents → Add New Agent**

### Agent 1 — Jose Perez
- Username: **jose.perez**
- Email: jose.perez@osticket.com
- Set password manually
- Assign:
  - **Department:** System Admin (Senior Admin)
  - **Team:** Level II Support

### Agent 2 — Richard Mills
- Assign:
  - **Department:** Support (View Only)

<br/>

<img src="https://i.imgur.com/QexHP1d.png"/>

---

## 🔹 Step 6 — Create Users
Switch to **Agent Panel**:

**Users → Create New User**

Create:

1. **Maria Larson** – maria.larson@osticket.com  
2. **John Wick** – john.wick@osticket.com  

<br/>

<img src="https://i.imgur.com/nqd72sj.png"/>

---

## 🔹 Step 7 — Configure SLAs
SLAs ensure timely ticket handling.

**Admin Panel → Manage → SLA → Add New SLA**

Create:

| SLA Name | Grace Period | Schedule |
|---------|--------------|----------|
| **SEV A** | 1 hour | 24/7 |
| **SEV B** | 4 hours | 24/7 |
| **SEV C** | 8 hours | Mon–Fri |

<br/>

<img src="https://i.imgur.com/Y0XNLPD.png"/>

---

## 🔹 Step 8 — Configure Help Topics
Help Topics streamline ticket categorization.

**Admin Panel → Manage → Help Topics → Add New Help Topic**

Create:

- Business Critical Outage  
- Personal Computer Issues  
- Equipment Request  
- Password Reset  

<br/>

<img src="https://i.imgur.com/aX2RVgn.png"/>

---

# 🎯 Skills Demonstrated
- Role-Based Access Control (RBAC)  
- Help Desk Administration  
- User & Agent Provisioning  
- Ticket Categorization  
- SLA Design & Prioritization  
- Workflow Optimization  

---

# 🏁 Completion Summary
You have successfully configured a fully functional osTicket support environment.  

This demonstrates your ability to:

- Administer enterprise support tools  
- Configure access controls  
- Build support workflows  
- Establish service-level expectations  
- Support real IT organizational structures  

These are the same skills expected of **IT Support**, **Help Desk**, and **Junior System Administrator** professionals.
