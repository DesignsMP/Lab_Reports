<h1>J. Q. Adams Case Study</h1>
  <h4>Objectives:</h4>
  <p>Our objective for this lab was to demonstrate all of the skills and techniques we covered in our System Administration class regarding group policies, DFS, Active Directory, and using requires for a company to meet their IT needs.
</p>
  <h4>Materials</h4> 
  <ul>
    <li>Pencil (to write down notes)</li>
    <li>Paper (to store notes)</li>
    <li>Remote Desktop (to communicate with rack server without having  to access it directly)</li>
    <li>Computers (to access applications such as Active directory)</li>
    <li>Draw.io (to create the diagram for our Active Directory structure)</li>
  </ul>
  <h4>Notes and Observations:</h4>
    <p>
      Test Text
    </p>
    <ol>
      <li> Our initial questions we would have asked the company towards the beginning of the project include:</li>  
      <ol>
          <li>What is the current structure organization?</li> 
          <li>What resources need to be shared and to whom?</li> 
          <li>What is the users home location?</li> 
          <li>What department is each employee a member of?</li> 
          <li>What is the business process and business goal?</li> 
          <li>Do they plan to grow in the near future?</li> 
          <li>What locations to users typically log in from?</li> 
          <li>How many subnets/ what is the IP address range?</li> 
          <li>What is the topology of their network?</li> 
          <li>What firewalls do they have in place?</li> 
      </ol>
<li> Some of the assumptions that were made for this cases study include: president was to be separate from vice presidents, I.S was to remain separate from the rest of the users, users should be placed under the server’s OU that they would use the most</li>
      <li> For file strucutre see attached document in the diagram section.</li> 
      <li> The naming policy for user accounts was the user’s first initial followed by their last name.  If they did not have a name it was the first initial for their department followed by employee and then an ID number.</li>
      <li> In order delegate control we right clicked on the production OU and chose the option to “delegate control.” From here we followed the steps in setting up the control such as what abilities are granted. In this case the vice president was to only have control over the user accounts in the OU and nothing else. The final step was to choose who received the delegate which was granted to AShinohara.</li>
      <li> When deciding on global and domain local groups we created a global group for each department. In the case for who had access to the AcctSys we created GG-Marketing, and GG-Accounting. These global groups were then put into the domain local group DL-Acct_Fin. We were later informed it is a better practice to name domain local groups after what they are providing access to.</li>
      <li> Some advantages of global groups include make managing users easy by having all users who need access to the same things all in one place. For example, all members in the accounting department needed access to the AcctSys application, so did the members of marketing, but they may still have different needs and so should be placed in separate global groups. In order to provide both access to the same application you simply put the global groups in a domain local group, which is specific to the application in question. From here the security settings would be edited to give the correct level of access to the groups with the domain local group.</li> 
      <li> It is important to use disk quotas because disk quotas keep the servers running smoothly, once too much memory is being used the system starts to slow down. It is very easy to use up too much space when you have a large number of employees all on the same servers.</li>
      <li> When it came to setting up the DFS we were unable to set it up due to a problem that occurred with a GPO. Once the error occurred all of our focus went to trying to fix the problem.</li>
      <li> Some of the advantages to using DFS include better organization of all files being shared throughout the business and namespaces make it easy to have access to all the necessary resources that appears as being all in one folder.</li>
      <li> When it came to group policies the way our group was setup I pretty much created all of the GPOs, Bryan was in charge of sharing files between users, and Matt was in charge of setting up the printer, downloading chrome enterprise, and attempted to create a second client computer.</li> 
      <li> Using the GPResult tool we are able to see which GPOs are currently in affect both for the computer settings and the user settings. This is important when either different users or computers need to have different GPOs in affect.</li>
      <li> When it came to Chrome Enterprise I am unsure how to do distribute it due to the fact that we installed chrome enterprise on a drive but did not distribute it to the client computer due to the issue we had with one of our GPOs. From what Matt told me it sounded like you would distribute it by first adding it to the Active Directory and then from there you would share it through a GPO.</li>
      <li> When it comes to roaming profiles, roaming profiles can be useful for those who work outside of the office. Through roaming profiles, although they may not be using a company owned computer, all of the same GPOs will be applied when the user logs into their account. This is very important when it comes to maintaining the security of a companies stored information.</li>
      <li> The biggest problem our group ran into we were never able to solve. Somehow, while I was limiting user’s access to the desktop, I blocked the use of the search bar and start menu. This became a crippling issue because it meant we could not test any of our GPOs that were to be applied to the users. To this day I still cannot think of any reason one of my GPOs would have blocked so much access without a probable cause. I checked all of my policies and reversed the only one I could think of that would have created these restrictions.</li> 
      <li> Conclusion can be found at the bottom of the page.</li>
    </ol>
  <h4>Diagrams, flowcharts, and figures:</h4>
  Here is an image to demonstrate how we set up our Active Directory structure and our file structure.
  <br><br><br>
 Active Directory Structure  
 
 ![Active Directory Structure](https://user-images.githubusercontent.com/31741807/58062539-4ce96b80-7b40-11e9-83ea-1e79ad6873a3.png)
 <br>File Structure
 
 ![File Structure](https://user-images.githubusercontent.com/31741807/58062625-95088e00-7b40-11e9-8812-ffa87487b91e.PNG)

  <h4>References:</h4>
    References for this lab include the case study and the tasks required to demonstrate our skills;
  
  
   [JQ Adams.pdf](https://github.com/DesignsMP/Lab_Reports/files/3200405/JQ.Adams.pdf)
   
   [lab_JQA_tasks.pdf](https://github.com/DesignsMP/Lab_Reports/files/3200406/lab_JQA_tasks.1.pdf)
   
   [Questions.pdf](https://github.com/DesignsMP/Lab_Reports/files/3200450/Report.pdf)

   
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> How did our OU structure look?</li>
  <li> How did our file strucutre look?</li>
  <li> Were you able to find out what was causing the issue with the client computer?</li>
  <li> What are some other programs you can distribute over active directory similar to chrome enterprise?</li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
    <p>
    In conclusion to this project I must first say this was a lot of fun. I was given the opportunity to use the knowledge I had learned from class and implement it as if I had earned an IT job at a company. I learned about the great tool of Active Directory to set up users, groups, and organizational units. I also learned about both the benefits and the consequences when using group policies to manage user’s and computer’s settings. If I were to do this project again, I would avoid creating any GPOs until I fully understood what the changes I have made would do. Even then I would still use it on a test computer/user to avoid ruining the current policies set in place for the company I am working for. Thanks for a great semester Mr. Harding. Hope my error leads to a hidden breakthrough that no one had found before.
    </p>

