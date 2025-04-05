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

<h2>Post-Install Configuration Objectives</h2>

- Acknowledge differences in agent & admin panels
- Configure roles, departments, teams, agents etc.
- Understand SLA management
- Create ticketing rules
- Configure topics for end users to place tickets

<h2>Configuration Steps</h2>

![image](https://github.com/user-attachments/assets/98fe4a78-c5a0-4614-8afc-401e0f5e7dfa)

<p>
Pull up both your admin/agent login page and your end user tiketing page to begin and login to your admin page with the credentials you selected
</p>
<br />

![image](https://github.com/user-attachments/assets/c8cab30e-6e42-4ff3-b485-68682325c6ca) ![image](https://github.com/user-attachments/assets/54c9e1c5-5398-4535-9825-b89151571b27)


<p>
First thing we will do is create a new role, be sure you are in the admin panel to perform this task, you can toggle back and forth by selecting the titled Agent panel/Admin panel next to Welcome "Your Name Here" at the top right of the page. Select Agents -> Roles -> Add new role. You may name it whatever you desire, I have named the new role "Supreme Admin" once named, go to the Permissions tab and check all permissions in Tickets, Tasks, & Knowledgebase and finally Add Role when complete
</p>
<br />

![image](https://github.com/user-attachments/assets/53db8705-36ab-417e-84ff-b52d18bc696f)

<p>
Next, let's create a department, select Agents -> Departments -> Add New Department, and we will create a "Top level department" named "SysAdmins" now select Create Department at the bottom of the page
</p>
<br />

![image](https://github.com/user-attachments/assets/9c1f1988-6765-43df-ae9d-72298cce8315)

<p>
Next I will create a team, select Agents -> Teams -> Add New Team, again this can be named whatever you desire, I have chosen "Online Banking" for this demonstration, select "Create Team"
</p>
<br />

![image](https://github.com/user-attachments/assets/74d28ba0-a6f2-4582-a344-bf571cb45a0d)

<p>
For the purposes of this demonstration we will be sure that there is no registration required in order to create tickets, so be sure under the settings tab that your page looks like the one pictured above.
</p>
<br />

![image](https://github.com/user-attachments/assets/c89a0028-ba7c-491f-9980-5a058e225cdc)

<p>
Now we will create some agents, be sure to note down the password you assign to your agent(s), under "Access" George will be "SysAdmins" and "Supreme Admin" role, "Permissions" will be left alone and "Teams" will be "Online Banking" now select create. Again we are going to create a second agent called James with a "support" position with "view only" access.
</p>
<br />

![image](https://github.com/user-attachments/assets/86767b63-0821-48f8-b6a3-8d0fa936283e)

<p>
Now we will create a user, enter the Agent Panel, select Users -> Add User and create a randomized user name and email, select Add user
</p>
<br />

![image](https://github.com/user-attachments/assets/913b224b-1af5-4264-b867-f167c0fcd9fa) ![image](https://github.com/user-attachments/assets/f4ccce25-e341-4951-9e91-4706fe36da89) ![image](https://github.com/user-attachments/assets/35115bcd-bcbf-4752-a7c5-8d86360bc37a)



<p>
Time to set up some Service Level Agreements (SLAs). Return to the Admin Panel select Manage -> SLA -> Add New SLA Plan and create a 3 SLAs titled Sev-A, B, & C as seen in the images above
</p>
<br />

![image](https://github.com/user-attachments/assets/c0976ab9-5eac-44a8-ada4-28e676d7c71d) ![image](https://github.com/user-attachments/assets/aec33ea3-3afb-433e-a167-350666fffd06)


<p>
Let's create multiple "Help Topics" Manage -> Help Topics -> Add New Help Topic, call these topics Business Critical Outage, Personal Computer Issue, Equipment Reset, Password Reset & Other. For these, assign a "Parent Topic" of either report a problem or general inquiry to organize them as you see fit for your project. Once completed you will see all Help Topics laid out as seen in the image above. This will conclude the post installation setup
</p>
<br />
