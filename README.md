<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<!-- <h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)
-->
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Step 1: Access the osTicket Admin & User Portals
- Step 2: Configure Roles (Permission Groups)
- Step 3: Configure Departments (Ticket Visibility)
- Step 4: Configure Teams
- Step 5: Allow Ticket Creation for Users
- Step 6: Configure Agents (Support Staff)
- Step 7: Configure Users (Customers)
- Step 8: Configure SLA (Service Level Agreements)
- Step 9: Configure Help Topics

<h2>Configuration Steps</h2>

<p>
## **Step 1: Access the osTicket Admin & User Portals**
<details>
<summary><b>Click to Expand</b></summary>

### **Login Pages**
- **Admin/Analyst Login Page**:  
http://localhost/osTicket/scp/login.php

markdown
Copy
Edit
- **End-User Portal**:  
http://localhost/osTicket

markdown
Copy
Edit

### **Agent Panel vs. Admin Panel**
- **Admin Panel**: For configuring settings, managing agents, and system-wide configurations.  
- **Agent Panel**: For managing tickets, responding to users, and handling support requests.  
</details>  
</p>
<br />

<p>
**Step 2: Configure Roles (Permission Groups)**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Agents** → **Roles**.  
2. Click **Add New Role** and create:  
 - **Supreme Admin** (Full permissions).  
</details>
</p>
<br />

<p>
 **Step 3: Configure Departments (Ticket Visibility)**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Agents** → **Departments**.  
2. Click **Add New Department** and create:  
 - **SysAdmins** (For IT System Administrators).  
 - **Networking** (For Network-related support).  
</details>
</p>
<br />

<p>
**Step 4: Configure Teams**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Agents** → **Teams**.  
2. Click **Add New Team** and create:  
 - **Online Banking** (Pulls agents from different departments).  
</details>
</p>
<br />

<p>
**Step 5: Allow Ticket Creation for Users**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Settings** → **User Settings**.  
2. **Uncheck**:  
 - ❌ "Unregistered users can create tickets."  
3. **Enable**:  
 - ✅ "Registration Required" (Users must register and log in to create tickets).  
</details>
</p>
<br />

<p>
**Step 6: Configure Agents (Support Staff)**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Agents** → **Add New**.  
2. Add the following agents:  
 - **Jane** (Department: SysAdmins).  
 - **John** (Department: Support).  
</details>
</p>
<br />

<p>
**Step 7: Configure Users (Customers)**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Agent Panel** → **Users** → **Add New**.  
2. Add the following users:  
 - **Karen**.  
 - **Ken**.  
</details>
</p>
<br />

<p>
  **Step 8: Configure SLA (Service Level Agreements)**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Manage** → **SLA**.  
2. Click **Add New SLA** and create:  
 - **Sev-A** (🚨 **Critical** – Grace Period: **1 hour**, Schedule: **24/7**).  
 - **Sev-B** (⚠️ **High** – Grace Period: **4 hours**, Schedule: **24/7**).  
 - **Sev-C** (📅 **Normal** – Grace Period: **8 hours**, Schedule: **Business Hours**).  
</details>
</p>
<br />

<p>
**Step 9: Configure Help Topics**
</p>
<p>
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Manage** → **Help Topics**.  
2. Click **Add New Help Topic** and create:  
 - 🛑 **Business Critical Outage**  
 - 💻 **Personal Computer Issues**  
 - 🏢 **Equipment Request**  
 - 🔑 **Password Reset**  
 - ❓ **Other**  
</details>
</p>
<br />

