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

<h2>If you need help installing osTicket follow my tutorial here</h2>

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents
- Configure Users
- Configure Service Level Agreements(SLA)
- Configure Help topics

<h2>Configuration Steps</h2>

<h2>Configure Roles</h2>

In the admin panel
- Select the Agents tab -> Roles -> Add New Role
	- Name : Supreme Admin
	- Select Permissions tab and check every box under the "Tickets", "Tasks" and "Knowledgebase" section
- Select Add Role
<p>
<img src="https://i.imgur.com/Dy6uQiW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Configure Departments</h2>

- In the admin panel
- Select the Agents tab -> Departments -> Add New Department 
	- Name: System Administrators
- Select Create Deptartment 
<p>
<img src="https://i.imgur.com/Q6eyyYZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/rjvmSSp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>	
	
<h2>Configure Teams</h2>

- In the admin panel
- Select the Agents tab -> Teams -> Add New Team
	- Name: Level II Support 
- Go to members tab and select yourself in "Select Agent" dropdown menu
- Select create team. 
<p>
<img src="https://i.imgur.com/ZVMQCgr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/obTQZlK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>	
	
<h2>Open Permissions to Allow Anyone to Create Tickets</h2>

 In the admin panel 
- Select the Settings -> User Settings
- Make sure box the "Registration Required: "Require registration and login to create tickets"is unchecked:  
<p>
<img src="https://i.imgur.com/wrnMuN9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>		
	
<h2>Configure Agents</h2>

-  In the admin panel 
- Select the Agents tab -> Add New Agents
	- Name: Jane Doe
	- Email : jane.doe@osticket.com
	- Username: jane.doe
	- Click set password and uncheck box that says "send the agent a password reset email
		- Set your password
		- uncheck "require password change at next login" box
		- set
<p>
<img src="https://i.imgur.com/IqORAgl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/c9AkP3L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

- Select Access tab 
	- Under Primary Department 
		- Select department dropdown menu -> System Administrators
		- Select Role dropdown menu -> Supreme Admin
	- Extended Accesss 
		- Select Department -> Support -> Add -> Supreme Admin
- Select Teams tab
	- Select team dropdown menu -> Level II Support
	- Select Add
- Select Create	

<p>
<img src="https://i.imgur.com/cT6DZrl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/9KosaQZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

- Create another agent named john and repeat the process again.
	- Follow same steps as above with some changes to Primary Department
		- Select department dropdown menu -> Support
		- Select Role dropdown menu -> View only
	- Extended Accesss 
		- Select Department -> Support -> Save Changes

<p>
<img src="https://imgur.com/cIc3Nhz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/c9AkP3L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



<h2>Configure Users</h2>

- In the Agent panel
- Select Users tab to create user
	- Email Address: Karen@osticket.com
	- Full Name - Karen Karen
	- Select Add User

<p align="center">
<img src="https://i.imgur.com/uDry69l.png" height="80%" width="80%" />

- Select user tab again to create another user
	- Email Address: Ken@osticket.com
	- Full Name - Ken Ken
	- Select Add User

<p align="center">
<img src="https://i.imgur.com/FploSL2.png" height="80%" width="80%" />


<h2>Configure Service Level Agreements(SLAs)</h2>

- In the admin panel 
- Select Manage tab -> SLA -> Add New SLA Plan 
	- Name: SEV-A 			
	- Grace Period: 1
	- Schedule dropdown menu: 24/7
	- Select Add Plan	
	
<p align="center">
<img src="https://i.imgur.com/RTQAZqQ.png" height="80%" width="80%" /> <img src="https://i.imgur.com/nLy3nPA.png" height="80%" width="80%" alt=/>
</p>

- Name: SEV-B
- Grace Period: 4
- Schedule dropdown menu: 24/7
- Select Add Plan
	
<p align="center">
<img src="https://imgur.com/GjQUZX8.png" height="80%" width="80%" />
</p>

- Name: SEV-C 
- Grace Period: 8
- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S Holidays
- Select Add Plan

<p align="center">
<img src="https://i.imgur.com/TPhqU1c.png" height="80%" width="80%" />
	

	
<h2>Configure Help Topics</h2>

- In the admin panel 
- Select Manage tab -> Help Topics -> Add New Help Topic 
	- Business Critical Outage
	- Personal Computer Issues
	- Equipment Request
	- Password Reset
- Select Add Topic for each topic

<p align="center">
<img src="https://i.imgur.com/uFmSyqK.png" height="80%" width="80%" />
<img src="https://i.imgur.com/PVlJh4x.png" height="80%" width="80%" />

And now everything is configured! :D
