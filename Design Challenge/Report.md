<h1>VLSM Design Challenge</h1>
  <h4>Objectives:</h4>
    The objective for this lab was to understand how VLSM subnetting work when it came to organizing and 
    utilizing all the available IP addresses when it came to distributing them out to companies in need of a network.
    
  <h4>Equipment List:</h4>
  <ul>
  <li>pencil (to write down notes)</li>
    <li>paper (to store notes)</li>
    <li>google docs (to create summary sheets with group editing capabilities)</li>
    <li>google sheets (to create the routing table with group editing capabilities)</li>
    <li>draw.io (to create the VLSM diagram with group editing capabilities)</li>
    <li>basecamp (to communicate with team members and to assign tasks)</li>
      </ul>
  
  <h4>Notes and Observations:</h4>
  When we started this project we went through three different models before we decided on one that would provide enough addresses to 
each company as well as keeping the amount of subnets at a minimum to prevent too much traffic. 
<ol>
<li>The first model was first split into two subnets. The first belonged entirely to the large company, the second subnet was split into four subnets. We kept a pattern of leaving subnet 0 empty, subnet 1 would belong to the next largest company, subnet 2 would be split into four more subnets, and subnet 3 would be left empty for future expansions. This pattern occured three times and provided each company with their own subnet.</li>
<li>The second model was similar to model one except for a few major differences. The major differences were the original IP was separated into four subnets rather than two to make room for more future expansions and each subnet used for the larger company was also the subnet separated into smaller subnets for the smaller companies. This model was ditched because at the time we could not figure out how to give the large companies the number of addresses the needed while still having enough left over for the smaller companies.</li>
<li>The third and final model was a combination of model 1 and model 2. We started with four subnets. We followed the same pattern as the smaller subnets from model 1 but we used it for all the subnets. Subnet 0 was empty, 1 for next largest company, 2 separated into four subnets for the smaller companies, 3 left empty for future expansion.</li>
  </ol>
  <h4>Diagrams, flowcharts, and figures:</h4>
  <ul>
    <li><a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Subnetting/Design%20Challenge/Design_Notes.png">Prototype Designs</a></li>
    <li><a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Subnetting/Design%20Challenge/Final_design.png">Final Network Diagram</a></li>
  </ul>
  <h4>References:</h4>
    The only references we had with this lab was information given to us in class. <a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Subnetting/Design%20Challenge/lab01_design_challenge.pdf">Lab_Worksheet</a>
  
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> How do companies know ahead of time how many IP addresses they will need to operate?</li>
  <li> Are there programs that make it easier to create routing tables?</li>
  <li> How to properly make a routing table?</li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
  From this lab I found out that subnetting is more complicated than I originally thought. I had never considered the possibility that you could take from one IP address and split it into smaller subnets in order to provide for multiple hosts. This is very beneficial when it comes to the limited amount of IP addresses available with IPv4 since it only has 32-bits. It is a great way to prolong our time until we have to switch to IPv6 which has 128-bits.
