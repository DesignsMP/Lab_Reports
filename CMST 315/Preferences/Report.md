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
      In this lab we were required to adjust policies and preferences on the computer's configuration rather than the user's configurations. First we created a new OU named "Local Computers" this way all of the computers can be linked to the computer configuration GPO's. Next we put our WinClient3A into the OU -> created two new GPO's named "Idle-time lockout Policy" and "Forced Applications" -> linked the two GPO's to the "Local Computers" OU. The GPO "Idle-time lockout Policy" would cause the screen to go to sleep after remaining inactive for sixty seconds. We set it up by naming it -> go into computer configurations -> under the polcies tab select windows settings -> select security settings -> select local Policies -> select security options -> choose "Interactive logon: Machine Inactivity limit" -> check off the "Define this policy setting" check box and define the number of seconds before going to sleep. Once this was completed we tested this on the client computer by logging in and waiting sixty seconds. The first time it did not work because we had forgotten to link the GPO to the "Local Computers" OU. After we linked it we tested it again and , as expected, the screen went black after sixty seconds of inactivity. Next we had to set up the "Forced Applications" GPO. We did this by selecting create new group policy object -> named it "Forced Applications" -> selected computer configuration -> selected policies -> selected administrative templates -> selected system -> selected logon -> chose the "Run these programs at User Logon" option -> enabled it and entered the program's paths so the computer could find the programs to open. We decided for the computer to open the calculator program and the notepad program. The path for the notepad program is "C:\Windows\System32\notepad.exe" and the path for the calculator program is "C:\Windows\system32\calc.exe" which was thankfully in the same directory. Once the paths were set we linked the GPO and tested it. The notepad program opened just fine but the calculator program never opened. After some troubleshooting we found that there was a space in the path causing it to not be found. Once the path was corrected we tested it again and both programs opened after a short loading time.
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
    In conclusion preferences and the computer's configuration are both efficiently powerful tools. The preferences can be used to set up GPO's that may be setting recommendations but the user does not necessarily have to follow them. The computer configuration settings make it easy to apply GPO's to all users by setting it to the device rather than to each individual user. Along with this it also makes it easier to know what kind of applications and policies are set on a specific device rather than trying to remember which users have access to which programs in a work or school environment. A perfect example would be the lab computers at school. It is far more efficient to control which applications are available on the computers in the labs than to set application permissions to the users based on their field of study.
    </p>
