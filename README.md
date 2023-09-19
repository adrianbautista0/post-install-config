<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Setup up Roles
- Create Departments
- Create Teams
- Allow users to create tickets
- Create Agents
- Create Users/Customers
- Create SLA plans
- Create Help Topics

<h2>Configuration Steps</h2>

If not already logged on from setting up osTicket in the previous section 
Go to the browser, paste this [link](http://localhost/osTicket/scp/login.php) and login in with your credentials 
When logged in, you will be at the agent panel 

### Setting Roles 

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/2caf34c7-9c66-4fb8-a1e5-eccfb9ce8bb7)


1. Admin panel > Go to Agents > Roles > Add New Roles
2. Name it “Supreme admin” or anything you want 
3. In permissions, check all the boxes in the Tickets, Tasks and Knowledgebase tabs 

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/f08eaf3c-2caf-4a9c-af94-328c4a663058)
![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/3321a0d2-f6c7-4851-8ebf-3916c803c2d0)
![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/4c8d277e-c3b2-48ef-b341-81022d324137)




4. Save changes when finished 
- For more information about roles, please visit this [page](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)

### Setting Departments  

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/003f1004-efa5-48bc-add5-14c825d8ca77)


1. Go to Agents > Departments > Add New Department 
2. For parent: Top Level Department 
- For the name: System Administrators 
- Leave the rest of the settings to default 
3. Then create department
- For more information about departments, please visit this [page](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)

### Setting Teams 

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/a122aa76-a46a-4ede-8555-2ab3b7b1427b)


1. Go to Agents > Teams > Add New Team 
2. Name the team: “Level II Support” 
- Leave the settings to default 
- Go to members tab and add yourself 
3. Create the team when finished
- For more information about teams, please visit this [page](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)

### Allowing people to create tickets 

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/6f74be62-ac6d-46d5-be9d-f16684633493)


1. Go to settings > Users > Settings 
2. Uncheck the box that says “Require registration and login in to create tickets” 
3. Save changes when finished 


### Setting up agents 
1. Agents > Add New Agent 
2. Name the agent “Jane Doe”
- Email address: put “janedoe@helper.com”
- Username: put “jane.doe”
- Set password 
- Uncheck the box that says “Send the agent a password reset email” 
- Write down the login credentials for this user 
- Uncheck box that says “Require password change at next login”
- Go to access tab > select System Administrators > select Supreme Admin Role 
- Go to teams tab > select Level II Support > create 

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/d91d5cbe-94d9-4983-b641-55303b04bc81)

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/e0744d19-499d-4ceb-8343-d4706568f508)


3. Repeat the same steps and create another agent 
- You can place this agent to be in different departments, roles, and teams as well. 
- For more information about Agents, please visit this [page](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)



### Setting up Users/Customers 
1. Switch to Agent Panel 
2. Go to Users > Add New User
3. Set an email and name then add user 

![image](https://github.com/adrianbautista0/post-install-config/assets/142345957/0ed4e550-fc6a-48f4-a9b8-e3dabcf5a3cf)


4. Repeat the same steps and add new user with a different name
- For more information about Users, please visit this [page](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html) 

### Setting up a SLA plan
1. Switch to Admin Panel 
2. Admin Panel > Manage > SLA > Add New SLA Plan 
- Name: “SEV-A”
- Grace Period 1
- Schedule 24/7
- Then add plan

- Add a New SLA Plan
- Name “SEV-B”
- Grace Period 4 
- Schedule 24/7
- Then add plan

- Add a New SLA Plan
- Name “SEV-C”
- Grace Period 8 
- Schedule Monday - Friday 8am - 5pm with U.S. Holidays 
- Then add plan
- For more information about SLA, please visit this [page](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html) 

### Configuring Help Topics 
1. Admin Panel > Panel > Help Topics 
- Select Add New Help Topic 
- Topic: Business Critical Outage 
- Save Changes 


- Select Add New Help Topic 
- Topic: Personal Computer Issues 
- Save Changes 


- Select Add New Help Topic 
- Topic: Equipment Reset 
- Save Changes 


- Select Add New Help Topic 
- Topic: Password Reset
- Save Changes 

- For more information about Help Topics, please visit this [page](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html) 

From sending a ticket as an end user to answering them as an agent or configuring the ticketing system as an administrator, you’ll get a basic understanding of how a ticketing system works.

