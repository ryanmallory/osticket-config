<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project outlines how to configure osTicket, an open-source help desk ticketing system. This process involves creating user and employee accounts, teams, departments, SLAs, permissions, and help topics.<br />

<h2>Technologies Used</h2>

- VMWare Workstation (Virtual Machine)
- osTicket (Help Desk Ticketing Software)
- Internet Information Services (IIS)

<h2>Operating System Used </h2>

- Windows 10 Pro</b> 

<h2>List of Configuration Parameters</h2>

- Roles
-  Departments 
-  Teams
-  Agents
-  Service Level Agreements (SLAs)
-  Help Topics
-  Users

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/rvxas5u.jpg" height="80%" width="80%"/>
</p>
<p>
In preparation of this lab, I installed osTicket on a Windows 10 virtual machine in VMWare Workstation. The installation process involved enabling/configuring Internet Information Services (IIS), setting up a MySQL database, and downloading many third-party programs. The picture above shows the default screen that opens when you login to osTicket's "admin" panel. In this lab, the majority of the configuration will take place in the admin panel.</p><br />

<p>
<img src="https://i.imgur.com/B2P6dHB.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/6A2cgtz.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 1: ROLES

Roles are the permissions granted to Agents (help desk employees) in a particular Department. Checking and unchecking different boxes determines how much administrative access an agent has while working with a ticket. In this example, I created a new role called "Level 1 Access". This role is designed for Tier 1 help desk agents and therefore has limited privileges. 
</p>
<br />

<p>
<img src="https://i.imgur.com/iBD5spp.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/SAUUStw.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 2: DEPARTMENTS

Creating Departments allows an organization to separate employees into logical groups. This makes it easy to route a ticket to every member of the support department, every member of the maintenance department, etc. I decided to create a new Department to hold all of the System Administrators.   
</p>
<br />

<p>
<img src="https://i.imgur.com/PzIeS9w.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/hoEEloM.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 3: TEAMS

Teams allow you to pull Agents from different Departments and group them together in order to handle a specific issue. For example, you could create a team called "Level II Support" and add one experienced Agent from each Department to the team.
</p>
<br />

<p>
<img src="https://i.imgur.com/ohZJGBU.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/jT7v5AJ.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/a6gLRwx.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 4: AGENTS

Agents are employees responsible for resolving and responding to tickets. Agents can be assigned to a Department and given Roles within that Department. For this project, I created 2 Agents: Jane Doe (a System Administrator), and John Doe (a Level I Support Technician).
</p>
<br />

<p>
<img src="https://i.imgur.com/tCwoYGC.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/voH0sPz.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 5: SERVICE LEVEL AGREEMENTS (SLAs)

Service Level Agreements are used to provide a length of time in which the help desk Administrator expects tickets to be closed. If a ticket were assigned a "SEV-1" (severity 1) SLA in the example above, that ticket would be expected to be closed within 4 hours regardless of the day or time (24/7). If the ticket isn't closed within 4 hours, it will be listed as overdue.
</p>
<br />

<p>
<img src="https://i.imgur.com/HicwN8f.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/LRSc119.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 6: HELP TOPICS

Help Topics help to streamline the process of creating tickets for end-users. If a User needed to have their password reset, they could simply select the Password Reset Help Topic and their ticket would be routed to the appropriate Department.
</p>
<br />

<p>
<img src="https://i.imgur.com/zwuTxNc.jpg" height="60%" width="60%"/>
</p>

<p>
<img src="https://i.imgur.com/W7lQo0Z.jpg" height="60%" width="60%"/>
</p>

<p>
STEP 7: USERS

Users are the people creating tickets in order to receive assistance from the help desk. When a ticket is created in the help desk, the user is associated with their email address in the User Directory of the help desk. For this lab, I created 2 Users, Sarah Smith and Jeff Jones.

In the next lab, I'll be using these User accounts to create tickets, and then I'll walk through the process of resolving and closing tickets as an Agent using all of the configuration settings created in this lab!
</p>
<br />
