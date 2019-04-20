<h1>Group Policy Management</h1>
  <h4>Objectives:</h4>
  <p>Our objective for this lab was to learn group policy terminilogy and to familiarize with the group policy management tools.
</p>
  <h4>Materials</h4> 
  <ul>
    <li>Pencil (to write down notes)</li>
    <li>Paper (to store notes)</li>
    <li>Remote Desktop (to communicate with rack server without having  to access it directly)</li>
    <li>Active Directory (to manage groups, users, computers, and other devices)
    <li>Computers (to access applications such as active directory)</li>
  </ul>
  <h4>Notes and Observations:</h4>
    <p>
    In this lab...
    </p>
    <ol>     
     <li> Its important to know how to use group policies when running an Active directory environment because...</li>
     <li> The levels of hierarchy in group policies are local domain, ...,..., Domain...</li>
     <li> The default domain policy GPO is initially in charge of ...</li>
     <li> The difference between a GPO being Not Configured compared to Disabled is...</li>
     <li> It is better to create GPO's rather than editing the default domain policy because with a GPO settings can be created for a specific user or computer, GPO's can be created for a specific set of settings, and it is easier to keep track of changes to a GPO rather than making all policy changes in a single location.</li>
     <li> As I said in the last response, it is best to keep the number of changes in a GPO to a minimum in order to keep track of all the changes/settings it would affect. If you have a GPO for each setting change, when you want to change that setting you would know exactly which GPO to modify.</li>
     <li> The purpose for gpudpate is to update the current user on the most recent GPO changes, and gpresult displays the GPO's that have been created and if they are in affect.</li>
     <li> One instance you would block GPO inheritance would be to  NOT DONE</li>
     <li> When a GPO is enforced it overrides any other GPO's in place dispite the level, if it is enforced it will only be overwritten if another GPO higher in the heirarchy is also enforced.</li>
     <li> User configuration settings would need to be disabled in the event of ...</li>
     <li> When testing new GPO's it is best to do it under an individual user or computer. In most cases people will create a user or computer specifically for testing. This is the best practice, that way if anything was wrong with the GPO it would not affect the whole system or all users. Once the bugs have been ironed out then they can distribute it out.</li>
     <li> BLocking any GPO with the deny permissions is very risky due to the inability for someone who has been denied to receive the GPO under any circumstances. If a group is denied, everyone in the group will be blocked.</li>
     <li> WMI filters can be used to filter ...</li>
    </ol>
  <h4>Diagrams, flowcharts, and figures:</h4>
  There were no diagrams or figures with this lab.
  <ul>
    
  </ul>
  <h4>References:</h4>
    References were both given in class and found online. This includes;
    <ul>
      <li> Names of computers and accounts</li>
      <li> IP Addresses</li>
      <li> Product Keys</li>
      <li> Passwords</li>
      <li> Mastering Windows Group Policy by Jordan Krause</li>
      <li>Group Policy by Jeremy Moskowitz</li>
    </ul>
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> </li>
  <li> </li>
  <li> </li>
  <li> </li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
    <p>
    In conclusion .
    </p>
