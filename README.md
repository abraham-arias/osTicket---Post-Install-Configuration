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

<h2>Tutorial Steps</h2>
<h3> Step 1: Configure Roles </h3> First, we are going to create a "Supreme Admin" role, and give this role full access. To do this from the Admin Panel we are going to "Agents", then "Roles", and "Add New Role". Enter the name "Supreme Admin". In Permissions, you are given different areas that you can assign permissions to this role. For this role we are going to check every permission, making this a role that can essentially do everything.
</p>
<br />
<img src="https://i.imgur.com/GCKAE7u.png" height="80%" width="80%" alt="Roles permissions"/>
</p>
<p>
<h3> Step 2: Configure Departments </h3> Next, we will create a department in the Admin Panel. Navigate to "Agents", "Departments", and select "Add New Department". Name this department "System Administrators", and for this project we are going to leave all the default settings and simply click "Create Department".
</p>
<br />
<img src="https://i.imgur.com/d0dogVG.png" height="80%" width="80%" alt="System Admins"/>
</p>
<p>
<h3> Step 3: Configure Teams </h3> Creating teams allows for multiple agents from different departments to collaborate together on a team. To make a team from the Admin Panel, navigate to "Agents", "Teams", and select "Add New Team". Call this team "Level II Support", and under the "Members" tab add yourself to the team.
</p>
<br />

<img src="https://i.imgur.com/P0wKPVo.png" height="80%" width="80%" alt="Level II Support"/>
</p>
<p>
<h3> Step 4: Allow Anyone To Create Tickets </h3> To do this in the Admin Panel, navigate to "Settings", "Users", "Settings", and uncheck "Require registration and login to create tickets".
</p>
<br />
<img src="https://i.imgur.com/rzXZ60d.png" height="80%" width="80%" alt="Anyone can create"/>
</p>
<p>
<h3> Step 5: Configure Agents </h3> Now we will create some agents, which are the help desk professionals who check and resolve tickets. In the Admin Panel, under "Agents", click "Add New Agent". The first agent will be named "Jane Doe" with an email of "jane.doe@osticket.com" and username "jane.doe". Make sure to note Jane's username for later. Click "Set Password", uncheck "Send the agent a password reset email", and enter a password for Jane. Once again, make note of this password for later. Uncheck "Require password change at next login", and click "Set". On the other tabs, this is where we can set Jane's permissions, add her to a team, and her department. Under "Access" We will put Jane in the "System Administrators" department as a "Supreme Admin". In "Teams" we will add her to "Level II Support", and then click "Create". Follow Step 5 to create a second agent with the name "John Doe". Set his department as "Support" and "View only". Now you should be able to see Jane and John under "Agents" with their departments listed.
</p>
<br />
<img src="https://i.imgur.com/trv3weH.png" height="80%" width="80%" alt="New agents"/>
</p>
<p>
<h3> Step 6: Configure Users </h3> Next, we will configure the users, who simply put, are the people opening tickets. To add users, switch to the "Agent Panel". Under "Users", click "Create New User". Name the first user "Karen Karen" with an email of "Karen@osticket.com", and "Add User". We will now add one more user. Following the same steps with the name Ken.
</p>
<br />
<img src="https://i.imgur.com/GFUOmmu.png" height="80%" width="80%" alt="New Users"/>
</p>
<p>
<h3> Step 7: Configure SLAs </h3> The purpose for the Service Level Agreement is to prioritize requests and also provide a length of time in which the help desk administrator expects the tickets to be resolved. So we will do this next. Go back to the "Admin Panel" and navigate to "Manage", and "SLA" where we will create 3 SLA plans. Click "Add New SLA Plan", naming it "SEV A", a grace period of "1" (hours), and schedule of "24/7". This means that at any time a ticket comes in, it has to be resolved in 1 hour. Next make two more SLAs, one called "SEV B", a grace period of "4" (hours), schedule of "24/7", and finally "SEV C", grace period of "8" (hours), schedule "Monday-Friday".
</p>
<br />
<img src="https://i.imgur.com/pnthCaA.png" height="80%" width="80%" alt="SLAs"/>
</p>
<p>
<h3> Step 8: Configure Help Topics </h3> Help topics help streamline tickets assignments for users, so we will configure a few now. In the Admin Panel, navigate to "Manage", "Help Topics", and click "Add New Help Topic". We will create the following 4 help topics: "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset".
</p>
<br />
<img src="https://i.imgur.com/N7dOIZu.png" height="80%" width="80%" alt="Help Topics"/>
</p>
<p>
<br />
<br/>
<h2> That completes the set up and configuration of osTicket! </h2>
