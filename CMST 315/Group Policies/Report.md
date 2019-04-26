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
    In this lab we set two goals in order to test our ability to control Group Policies. The first was to set the wallpaper for all members in our Main Organizational Unit. Our group decided to take it a step further and set a different wallpaper for each OU within our Main OU. To create a new GPO we opened the Server Manager -> open tools -> select group policy management. From here we clicked on Group Policy Objects -> create new GPO -> named it "Set Wallpaper to Shockwave -> went to User Configuration -> Administration Template -> Desktop -> Desktop -> Desktop Wallpaper -> Select Enable -> insert path "\\WINSERVER3B\Wallpaper\Shockwave Wallpaper.png" -> selected style to "fit". We then had the link the OU by first selecting the Marketing OU under Main -> right clicked -> select "Link an Existing GPO" -> selected "Set Wallpaper to Shockwave" and then tested the connection.
    </p>
    <ol>     
     <li> Its important to know how to use group policies when running an Active directory environment because its the technique used to provide security and to make sure users have access to the applications they need and do not have access to applications they do not need. It also helps organize a companies file sharing access in order to spread information over a large number of people.</li>
     <li> The levels of hierarchy in group policies are local policies, Site policies, Domain policies, and Organizational Unit policies. These work together by policies being set locally either by the user or computer are read first, these would then be overwritten for any policies written for a specific site, if the structure included any, next the domain's policies would be set next and overwrite any of the previous policies, finally any policies set for a specific organizational unit will overwrite all previous policies written.</li>
     <li> The default domain policy GPO is initially in charge of all users in the domain, it is typically used to control password and other security policies.</li>
     <li> The difference between a GPO being Not Configured compared to Disabled is when a person sets a GPO to disabled then the settings that would be affected will be restored to default behavior. If the GPO is not configured then the system knows you haven't decided on those specific settings and will check elsewhere to see if another GPO has changes to those settings.</li>
     <li> It is better to create GPO's rather than editing the default domain policy because with a GPO settings can be created for a specific user or computer, GPO's can be created for a specific set of settings, and it is easier to keep track of changes to a GPO rather than making all policy changes in a single location.</li>
     <li> As I said in the last response, it is best to keep the number of changes in a GPO to a minimum in order to keep track of all the changes/settings it would affect. If you have a GPO for each setting change, when you want to change that setting you would know exactly which GPO to modify.</li>
     <li> The purpose for gpudpate is to update the current user on the most recent GPO changes, and gpresult displays the GPO's that have been created and if they are in affect.</li>
     <li> One instance you would block GPO inheritance would be to if a specific department, such as IT, do not need to be held under the firewall. They would create a GPO for the firewall settings, link it to the domain, and block inheritance to the IT OU so they can continue working on things the firewall would normally block.</li>
     <li> When a GPO is enforced it overrides any other GPO's in place dispite the level, if it is enforced it will only be overwritten if another GPO higher in the heirarchy is also enforced.</li>
     <li> User configuration settings would need to be disabled in the event of ...</li>
     <li> When testing new GPO's it is best to do it under an individual user or computer. In most cases people will create a user or computer specifically for testing. This is the best practice, that way if anything was wrong with the GPO it would not affect the whole system or all users. Once the bugs have been ironed out then they can distribute it out.</li>
     <li> BLocking any GPO with the deny permissions is very risky due to the inability for someone who has been denied to receive the GPO under any circumstances. If a group is denied, everyone in the group will be blocked.</li>
     <li> WMI filters can be used to filter GPO's even further by looking at information available on the computer and seeing if the GPO meets the criteria. An example of this would be for a GPO to only be enforced if a computer has more than ten gigabytes of available space.</li>
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
      <li> Group Policy by Jeremy Moskowitz</li>
    </ul>
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> Are there any instances when a company would have Active Directory but not use group policies?</li>
  <li> Are there other programs to choose from for this type of application besides Active Directory></li>
  <li> What was the common practice when it came to sharing files and enforcing rules before Active Directory was implemented?</li>
  <li> Due to how strong the consequences are, what is the best practice for denying sharing permissions?</li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
    <p>
    In conclusion .
    </p>
