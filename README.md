<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- OsTicket Installed
- Internet Information Services (IIS)
<h2>Operating Systems Used </h2>

- Windows 10 Pro </b> (22H2) at Least 2vCPUs and 8 GB RAM

<h2>Post-Install Configuration Objectives</h2>

- Configuring Roles, departments, and teams

- Configuring Agents "employees" and Users "customers"
  
- Configuring SLA's (service level agreements)<br />
  
   <b>Sev-A</b> (Grace Period) 1hr/ schedule 24/7
  
   <b>Sev-B</b> (Grace Period) 4hr/ schedule 24/7
  
   <b>Sev-C</b> (Grace Period) 8hr/ schedule Business Hours Only
  
- Configuring Help Topic/s

<h2>Role Configuration Steps</h2>
<p> Log in as Admin user to http://localhost/osTicket/scp then click on Admin Panel in the top right/ Agents tab, to bring up Roles / Select Roles
  </p>
<br />

![1st](https://github.com/user-attachments/assets/8f9b90f7-feaf-4712-9db1-d6bd3834f110)

</p>
<p>
<h2></h2>
Each role allows for different permissions for the agents being created. They range from View only, which means the agent can only View Tickets and nothing else, to All Access, which provides unlimited access and can allow an agent to assign tickets to others, change SLA levels, create, close, and delete tickets. 
</p>


![2nd](https://github.com/user-attachments/assets/bd18738b-d504-45b2-8270-54d0f8043923)
<h2></h2>
Selecting "Departments" next to the Roles tab, then Add new department, will bring up the following menu. This section allows us to create different departments within the company, set different SLA schedules, allow tickets to be assigned to certain departments, and send alerts and autoresponses. 

<p>
  
![3rd](https://github.com/user-attachments/assets/2bf5121d-3876-496b-9061-02dcfd4bc15d)
<h2></h2>
</p>
<p>

</p>
<br />

<p>
We can create teams within departments to help categorize the different roles of our agents. For example, we can create an Online Banking team with the SysAdmins department. Then, we may also add Members within the team to respond to tickets. Although we can only do this once we've created the agents.
 
  We can also allow users to create tickets without having to register for an account for our help desk. Click on Settings/ Users/ Uncheck Require registration and login to create tickets option. This will make it easier for users to get IT support.
  
  ![4th](https://github.com/user-attachments/assets/082005d6-8d98-4ef5-a2e1-84cd387f58ae)
<h2></h2>
</p>

<p>
Now we can create some agents to work on our tickets. Click on Agents (big tab) / Add New Agent.

  ![5th](https://github.com/user-attachments/assets/0f32b5ab-d86c-44f4-b9f7-92d4c9e2a61c)

</p>
<h2></h2>
<p>
We can set an agent's name, password, email address, access, permissions, and which team they'll be on. For example, we can create an agent named Jane Doe and assign her to the SysAdmins department and give her All Access. We can also create another user named John Doe and assign him to the Support department and provide him with Expanded Access. Setting the access will also set the preconfigured permissions, but you can also fine-tune certain permissions. 

  ![6](https://github.com/user-attachments/assets/b98f6d46-69fe-4d56-af0a-97a6420e2c70)
<h2></h2>
</p>

<p>

</p>
<br />
 To assign each agent to specific teams to allow them to assign tickets to other agents from other teams if needed. Simply click on Teams and add each agent to their required team. In this instance, we'll assign Jane Doe to Online Banking and John Doe to Support.
<p>
<img src="https://i.imgur.com/b5WfIq1.png" height="80%" width="80%" alt="setting agents access"/>
<img src="https://i.imgur.com/dfg5fLP.png" height="80%" width="80%" alt="john and jane doe agents"/>
  
<h2></h2>

</p>

<p>


We can also create users (customers) who need support. To do that, click on the Agent Panel at the top right, then click on Users, then Add User. In this example, we can create 2 users named Karen and Ken.

</p>
<br />
<p>
  <img src="https://i.imgur.com/kKMGzST.png" height="80%" width="80%" alt="creating users"/>
</p>
<h2></h2>
<p>
It's also important that our agents can work through the tickets according to how important or urgent it is based on business impact. We can do this by creating differing SLA (service level agreement) levels.
  
  Click on Add New SLA plan, we can add in the details for our SLAs based on severity (Sev-A being most urgent to Sev-C being least urgent). We want to set it like this <b>Sev-A</b> (grace period: 1hr, schedule: 24/7), <b>Sev-B</b> (grace period: 4hr, schedule: 24/7), <b>Sev-C</b> (grace period: 8hr, schedule: Business hours). 
</p>
<br />
<p>
  <img src="https://i.imgur.com/n476nPM.png" height="80%" width="80%" alt="creating SLA"/>
</p>

<p>

<h2></h2>
Finally, we can also create different help topics to allow tickets to be sent in the right category for our agents to work through. In reality, we will likely have to reassign the ticket to a more appropriate help topic, as users don't usually choose the best one. But it's good to have options! 
</p>
<br />

<p>
<img src="https://i.imgur.com/3cRwV9i.png" height="80%" width"80%" alt="create help topics"/>
</p>
<p>
We can now create different help topics and choose a top-level topic, like Report a Problem, to create a more specific help topic within this area, like an Access Issue. By clicking on the Admin Panel at the top, then Manage, and then Add New Help Topic
</p>
<br />
<b>Thank you for following along!</b>
</p>
