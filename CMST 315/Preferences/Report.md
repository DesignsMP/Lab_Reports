<h1>Deploying Preferences</h1>
  <h4>Objectives:</h4>
  <p>Our objective for this lab was to familiarize ourselves with the actual settings within Group Policy Objects.
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
    </p>
    <ol>
     <li> The main differences between a GPO policy and a preference is the fact that policies can disable certain applications and settings for users, meanwhile a preference would hide those settings but the user could re-enable them if they so choosed. Another would be that policies can be set at both the domain and local level while preferences can only be set at the domain level.</li>      
     <li> The administrative templates are more flexible than other group policies due to the fact that they pull information from templates on the local computer. Whenever policies are changed those changes are stored in a register key this way all changes are implemented as soon as the computer refreshes.</li>
     <li> Some of the computer configuration settings that can be changed would include:
          <ul>
            <li> Having specific applications open upon login</li>
            <li> Control a screen based on idle time</li>
          </ul>
     </li>
     <li> Some of the user configuration settings that can be changed would include:
          <ul>
            <li> Having specific backgrounds apply to an OU or User</li>
            <li> Require a password change after a specified amount of time</li>
          </ul>
     </li>
    </ol>
  <h4>Diagrams, flowcharts, and figures:</h4>
  Here are some figures that were mentioned in the observations.
  
    
   ![Lab 7 lines](https://user-images.githubusercontent.com/31741807/56866655-59473200-69a1-11e9-83ca-e9f235bce689.png)
   <p>Lines that if green would push preferences to the computer, and if red would not manipulate any settings.</p>
   
   ![Lab 7 Idle](https://user-images.githubusercontent.com/31741807/56866656-59dfc880-69a1-11e9-90af-aa6d3c204d1f.png)
   <p>Screen viewed when enabling the computer screen to go to sleep if activity was idle for 60 seconds.</p>
    
  <h4>References:</h4>
    References were both given in class and found online. This includes;
    <ul>
      <li> Mastering Windows Group Policy by Jordan Krause</li>
    </ul>
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> Which user configuration settings are typically left as preferences rather than actual policies?</li>
  <li> What are some examples of computer configuration settings? I'm sure there's a lot more than what we had mentioned in class.</li>
  <li> Can the computer configuration settings be used to optimize the computers performance?</li>
  <li> What is the easiest way to keep track of all of the policies and preferences created in a workplace environment? Do they typically have the two separated?</li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
    <p>
    In conclusion .
    </p>
