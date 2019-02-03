VLSM Design Challenge
  Objectives:
  <br>
    The objective for this lab was to understand how VLSM subnetting work when it came to organizing and 
    utilizing all the available IP addresses when it came to distributing them out to companies in need of a network.
    
  Equipment List:
  <br>
  <ul>
  <li>pencil (to write down notes)</li>
    <li>paper (to store notes)</li>
    <li>google docs (to create summary sheets with group editing capabilities)</li>
    <li>google sheets (to create the routing table with group editing capabilities)</li>
    <li>draw.io (to create the VLSM diagram with group editing capabilities)</li>
    <li>basecamp (to communicate with team members and to assign tasks)</li>
      </ul>
  
  Notes and Observations:
  <br>
  When we started this project we went through three different models before we decided on one that would provide enough addresses to 
each company as well as keeping the amount of subnets at a minimum to prevent too much traffic. 
<ol>
<li>The first model was first split into two subnets. The first belonged entirely to the large company, the second subnet was split into four subnets. We kept a pattern of leaving subnet 0 empty, subnet 1 would belong to the next largest company, subnet 2 would be split into four more subnets, and subnet 3 would be left empty for future expansions. This pattern occured three times and provided each company with their own subnet.
<li>The second model was similar to model one except for a few major differences. The major differences were the original IP was separated into four subnets rather than two to make room for more future expansions and each subnet used for the larger company was also the subnet separated into smaller subnets for the smaller companies. This model was ditched because at the time we could not figure out how to give the large companies the number of addresses the needed while still having enough left over for the smaller companies.
<li>The third and final model was a combination of model 1 and model 2. We started with four subnets. We followed the same pattern as the smaller subnets from model 1 but we used it for all the subnets. Subnet 0 was empty, 1 for next largest company, 2 separated into four subnets for the smaller companies, 3 left empty for future expansion.
  
  Diagrams, flowcharts, and figures:
    <a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Subnetting/Design%20Challenge/Final_design.png">Network Diagram
  
  References:
  
  Questions:
  
  Conclusion and Reflection:
  
