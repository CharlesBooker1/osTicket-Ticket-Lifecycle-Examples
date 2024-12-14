<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Understanding the Ticket Lifecycle</h1>
This guide explains the ticket lifecycle within the open-source help desk system osTicket, from ticket creation to resolution. It is assumed that you have already completed the <a href="">installation</a> and <a href="">configuration</a> of osTicket.

</br>

<h2>Technologies and Environments Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
  <li>osTicket</li>
</ul>

</br>

<h2>Operating System Used</h2>
<ul>
  <li>Windows 10</li>
</ul>

</br>

<h2>Ticket Lifecycle Phases</h2>
<ol>
  <li>Ticket Intake</li>
  <li>Assignment and Communication</li>
  <li>Issue Resolution</li>
  <li>Closing the Ticket</li>
</ol>

</br>

<h2>Lifecycle Overview</h2>

<h3>Ticket Intake</h3>

<p>
  <ul>
    <li>The process begins with the <b>End User</b> (e.g., Karen) creating a new ticket through the <a href="http://localhost/osTicket/">local osTicket site</a>. The user enters their details and selects a Help Topic.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/96bb4609-e295-4fd2-aa54-a32edb81c2d5" height="80%" width="80%" alt="Ticket Intake Screenshot"/></li>
    </ul>
    <li>Next, the End User provides a description of the issue in the <b>Issue Summary</b>, similar to composing an email.</li>
    <ul>
      <li>For this example, Karen reports a 404 error in the mobile banking app under the "Business Critical Outage" help topic (configured in osTicket).</li>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/b8642323-ce9f-4f42-9b44-960304f81486" height="80%" width="80%" alt="Ticket Submission Screenshot"/></li>
    </ul>
    <li>Once the ticket is created, it is forwarded to <b>Agent</b> Jane Doe (the Supreme Admin, who can view all incoming tickets, as set up in the configuration tutorial) for review via the <a href="http://localhost/osTicket/scp/login.php">local help desk login</a>.</li>
    <ul>
      <li><b>Note:</b> At this stage, other tickets, like #951342 from Ken, requesting an Adobe Reader upgrade, are not yet prioritized. SLA plans need to be configured for these requests, so all tickets are marked with a "Normal" priority.</li>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/01887ba4-d7c5-4c9b-8890-9ffc02f350a4" height="80%" width="80%" alt="Ticket Review Screenshot"/></li>
    </ul>
  </ul>
</p>

<h3>Assignment and Communication</h3>

<p>
  <ul>
    <li>Once ticket #282733 (Business Critical Outage) is assigned to Agent Jane Doe, it appears in her dashboard as shown below.</li>
    <ul>
      <li>From here, the Agent can initiate communication with the End User using the <b>Ticket Thread</b> at the bottom of the page.</li>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/dad0149d-9a9a-427a-88e7-73a91ee3bcd3" height="80%" width="80%" alt="Ticket Thread Screenshot"/></li>
    </ul>
    <li>The priority of the ticket can be set by selecting a level (Low, Normal, High, Emergency) from the <b>Priority</b> section.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/aceb0b2b-6d14-486c-951b-5510c01288d3" height="80%" width="80%" alt="Priority Setting Screenshot"/></li>
    </ul>
    <li>The ticket can also be assigned to different teams or agents by selecting the <b>Assigned to</b> field. If the ticket is assigned to an agent outside of Jane's department, it will not appear in her feed.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/7705f431-b2b8-4a70-b357-cb9099276909" height="80%" width="80%" alt="Assign Ticket Screenshot"/></li>
    </ul>
    <li>The <b>SLA Plan</b> can be adjusted to match predefined plans, such as SEV-A, for urgent tickets like this one.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/b088102b-45e2-4303-b557-12df0c70eb48" height="80%" width="80%" alt="SLA Plan Setting Screenshot"/></li>
    </ul>
    <li>Finally, the <b>Department</b> field is set, changing the ticket's assignment from Support to System Administrators for this critical issue.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/9fe7f262-9961-4ab9-b95c-c1a0c13be6a5" height="80%" width="80%" alt="Department Setting Screenshot"/></li>
    </ul>
    <li>All updates to the ticket will be visible in the Ticket Thread.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/d69cf505-0e4d-4616-9718-8cdc823ea154" height="80%" width="80%" alt="Ticket Thread Updates Screenshot"/></li>
    </ul>
    <li>The Agent can then send messages to the End User and adjust the ticket's status (left as <b>Open</b> for now).</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/becb0089-d4b7-411f-bba0-d5e5fefd649b" height="80%" width="80%" alt="End User Message Screenshot"/></li>
    </ul>
  </ul>
</p>

<h3>Issue Resolution and Ticket Closure</h3>

<p>
  <ul>
    <li>After collaborating with the System Engineering team, the issue in the Critical Banking Outage ticket has been resolved. The Agent updates the End User through the Ticket Thread and changes the status from Open to <b>Resolved</b>. The ticket is then <b>Closed</b> after the final reply.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/fa08856b-4eb5-430b-ac76-ca606e494229" height="80%" width="80%" alt="Ticket Resolution Screenshot"/></li>
    </ul>
    <li>Closed tickets are archived in the Closed section of the Tickets tab. It is a best practice for Agents to review these tickets to improve their handling of similar issues in the future.</li>
    <ul>
      <li><img src="https://github.com/ColtonTrauCC/ticket-lifecycle/assets/147654000/2e3b4963-5ca7-4d82-a004-17d2c166c8a0" height="80%" width="80%" alt="Closed Ticket Screenshot"/></li>
    </ul>
  </ul>
</p>

<br />
