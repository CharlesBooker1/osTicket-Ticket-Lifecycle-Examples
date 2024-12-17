<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Ticket Lifecycle</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket. This tutorial assumes you have completed both the installation and configuration of osTicket<br />
</p>
<p>
<h3>Environments and Technologies Used</h3>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h3>Operating Systems Used </h3>

- Windows 10</b>

<h3>Ticket Lifecycle Stages</h3>
<p>
<ol>
  <li>Intake</li>
  <li>Assignment & Communication</li>
  <li>Working the Issue</li>
  <li>Resolution</li>
</ol>
<p>
<h3>Lifecycle Stages</h3>
<h3>Intake</h3>

<p>

<p>
From the End Users side (Karen Smith), they create a ticket through osTickets local host site and fill their information. Select a Help Topic.
</p>
<img src="https://i.imgur.com/4ujArW4.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
</p>
<p>
The End User then writes ticket through the Issue Summary and adds a subject and details of the ticket much similiar to writing an email. 
</p>
In this example, Karen creates the ticket under the Help Topic of a Business Critical Outage, explaining the mobile baking operation is suffering a 404 error
</p>
<p>
<img src="https://i.imgur.com/RKfGwrM.png" height="55%" width="55%" alt="Disk Sanitization Steps"/>
</p>
<p>
Karen then creates the ticket and is sent to Agent Jane Doe (which we've set as Supreme Admin is able too see all incoming tickets in the configuration tutorial) who views it from the local help desk login
<p>
Priorities have not been set for other incoming tickets such as ticket #174883 where end user Ken is requesting an upgrade to Adobe Reader. SLA plans need to be set for these tickets hence why they are all under the priority state of "Normal"
</p>
<img src="https://i.imgur.com/O04oImP.png" height="65%" width="65%" alt="Disk Sanitization Steps"/>
</p>
</ul>
</p>

<h3>Assignment & Communication</h3>

</p>

<p>
The Business Critical Outage ticket by Karen numbered #903656 is assigned to the Agent Jane Doe. From Jane's perspective, this is how the ticket first looks. The Agent is able to message the End User through the Ticket Thread located in the bottom of the ticket page
</p>
<img src="https://i.imgur.com/V1FumyE.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
By going to the link next to Priority, you are able to set the priority of the ticket to Low, Normal, High, or Emergency. As an example set this to Emergency, add in the notes business impacting event.
<p>
<img src="https://i.imgur.com/ffz92Hd.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
By going to the Assigned To option, you can assign the ticket to a Team or Agents. Assign the role to Jane Doe
<img src="https://i.imgur.com/4p3JJUu.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
By going to the link next to SLA Plan to set the SLA Plan from Default SLA to one of our SLA Plans we have created in configuration. For this Business Critical Outage ticket, it'll be set to SEV-A. In the notes add business impacting, critical incident.
</p>
<img src="https://i.imgur.com/ioWM91F.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
By going to the link next to Department to set the Department. For this Business Critical Outage ticket, it'll be set from Support to System Administrators. Add in the notes Sys Admins responsible for mobile banking infrastructure
</p>
<img src="https://i.imgur.com/YzoWRLP.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
The Ticket Thread section displays the updated information when we make changes to the ticket
</p>
<img src="https://i.imgur.com/OtLtJ3E.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
The Agent can message the End User through the Ticket Thread to update the User on the ticket as well as set the status of the ticket (which is left as Open since we need to work it out)
</p>
<img src="https://i.imgur.com/9YUHdxc.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
</ul>
</p>

<br />

<h3>Working the Issue and Resolution</h3>

<p>

Proceeding from the last section, the issue in our hypothetical Critical Banking Outage ticket has been resolved from the System Engineering department. The Agent should communicate with the End User using the Ticket Thread and set the status of the ticket from Open to Resolved. After posting the reply the ticket is closed.
</p>
<img src="https://i.imgur.com/ESXASE8.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
Closed tickets can be found under the closed section in our Tickets tab, where information and status of the tickets are archived.
</p>
<img src="https://i.imgur.com/9XKpQXd.png" height="65%"  width="65%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />
This is the conclusion of the lab
