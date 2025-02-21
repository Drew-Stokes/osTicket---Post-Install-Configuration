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
- Step 5: Configure Agents (Support Staff)
- Step 6: Configure Users (Customers)
- Step 7: Configure SLA (Service Level Agreements)
- Step 8: Configure Help Topics


<h2>Configuration Steps</h2>

<p>
## **Step 1: Access the osTicket Admin & User Portals**
<details>
<summary><b>Click to Expand</b></summary>

### **Login Pages**
- **Admin/Analyst Login Page**:  
http://localhost/osTicket/scp/login.php
<p/>
<img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/10439022fd8100b61b32e16ffa1b420a86c17da3/osTicket_admin_login.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>


- **End-User Portal**:  
http://localhost/osTicket
<p/>
<img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/10439022fd8100b61b32e16ffa1b420a86c17da3/osTicket_endUser_login.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>

### **Agent Panel vs. Admin Panel**
- **Admin Panel**: For configuring settings, managing agents, and system-wide configurations.
  <p>
  <img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/45e81b944c41633c2b56d18666f3f6c95094ac68/osTicket_Admin_panel.png" height="30%" width="30%" alt="Disk Sanitization Steps"/> 
  </p>
- **Agent Panel**: For managing tickets, responding to users, and handling support requests.
  <p>
  <img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/45e81b944c41633c2b56d18666f3f6c95094ac68/osTicket_Agent_panel.png" height="30%" width="30%" alt="Disk Sanitization Steps"/> 
  </p>
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
   <p/>
<img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/1f44685b4b26bc7d0be078d2f0a151e0f5742df3/supreme_admin.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>
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
   <p>
  <img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/d22ed5aa9612d318a01bdf474ddcc909d1028a6a/sysadmins.png" height="30%" width="30%" alt="Disk Sanitization Steps"/> 
  </p>  
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
   <p>
  <img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/7110f415f792dd0329015a36c16b495f2c31f629/online_banking.png" height="30%" width="30%" alt="Disk Sanitization Steps"/> 
  </p>  
</details>
</p>
<br />

<p>
**Step 5: Configure Agents (Support Staff)**
<details>
<summary><b>Click to Expand</b></summary>

1. Navigate to **Admin Panel** → **Agents** → **Add New**.  
2. Add the following agents:  
 - **Jane** (Department: SysAdmins).
   <p>
  <img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/fbb5cfc68a037dcdc79784785f0f23a6dfe74482/jane_sysadmin.png" height="30%" width="30%" alt="Disk Sanitization Steps"/> 
  </p>   
 - **John** (Department: Support).  
 <p>
  <img src="https://github.com/Drew-Stokes/osTicket---Post-Install-Configuration/blob/fbb5cfc68a037dcdc79784785f0f23a6dfe74482/john_new_agent.png" height="30%" width="30%" alt="Disk Sanitization Steps"/> 
  </p>  
</details>
</p>
<br />

<p>
**Step 6: Configure Users (Customers)**
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
**Step 7: Configure SLA (Service Level Agreements)**
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
  **Step 8: Configure Help Topics**
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

