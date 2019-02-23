<h1>Virtual Windows Server</h1>
  Objectives:
  <br>
    The objective for this lab was to understand virtual machines and servers and how they allow you to run several different machines all on one computer or server. With the possibility it also allows people to have multiple machines each with the ability to be customized to a specific need without affecting any of the other virtual machines.
    
  Equipment List:
  <br>
  <ul>
    <li>Pencil (to write down notes)</li>
    <li>Paper (to store notes)</li>
    <li>Hyper-V (to manage all of our virtual machines)</li>
    <li>Dell rack server (to store and run all of our virtual machines)</li>
    <li>Windows Server 2016 (the purpose of the virtual server and tool for the next lab)</li>
    <li>Remote Desktop (to communicate with rack server without having  to access it directly)</li>
  </ul>
  
  Notes and Observations:
  <br>
  When we started this project we went through three different models before we decided on one that would provide enough addresses to 
each company as well as keeping the amount of subnets at a minimum to prevent too much traffic. 
<ol>
<li>The first model was first split into two subnets. The first belonged entirely to the large company, the second subnet was split into four subnets. We kept a pattern of leaving subnet 0 empty, subnet 1 would belong to the next largest company, subnet 2 would be split into four more subnets, and subnet 3 would be left empty for future expansions. This pattern occured three times and provided each company with their own subnet.</li>
<li>The second model was similar to model one except for a few major differences. The major differences were the original IP was separated into four subnets rather than two to make room for more future expansions and each subnet used for the larger company was also the subnet separated into smaller subnets for the smaller companies. This model was ditched because at the time we could not figure out how to give the large companies the number of addresses the needed while still having enough left over for the smaller companies.</li>
<li>The third and final model was a combination of model 1 and model 2. We started with four subnets. We followed the same pattern as the smaller subnets from model 1 but we used it for all the subnets. Subnet 0 was empty, 1 for next largest company, 2 separated into four subnets for the smaller companies, 3 left empty for future expansion.</li>
  </ol>
  Diagrams, flowcharts, and figures:
  <br>
  <ul>
    <li><a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Subnetting/Design%20Challenge/Design_Notes.png">Prototype Designs</a></li>
    <li><a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Subnetting/Design%20Challenge/Final_design.png">Final Network Diagram</a></li>
  </ul>
  References:
  <br>
    The only references we had with this lab was information given to us in class. This includes;
    <ul>
      <li> Names for the computers and accounts</li>
      <li> IP address information</li>
      <li> Product keys</li>
      <li> Passwords</li>
    </ul>
  Questions:
  <br>
  A few things I am still confused on are:
  <ol>
  <li> How do companies know ahead of time how many IP addresses they will need to operate?</li>
  <li> Are there programs that make it easier to create routing tables?</li>
  <li> How to properly make a routing table?</li>
  </ol>
  Conclusion and Reflection:
  <br>
  From this lab I found out that subnetting is more complicated than I originally thought. I had never considered the possibility that you could take from one IP address and split it into smaller subnets in order to provide for multiple hosts. This is very beneficial when it comes to the limited amount of IP addresses available with IPv4 since it only has 32-bits. It is a great way to prolong our time until we have to switch to IPv6 which has 128-bits.
