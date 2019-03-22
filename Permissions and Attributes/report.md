<h1>Permissions and Attributes</h1>
  <h4>Objectives:</h4>
  <p>Our objective for this lab was to use Active Directory to manage the permissions and attributes.
</p>
  <h4>Materials</h4> 
  <ul>
    <li>Pencil (to write down notes)</li>
    <li>Paper (to store notes)</li>
    <li>Remote Desktop (to communicate with rack server without having  to access it directly)</li>
    <li>Active Directory (to manage groups, users, computers, and other devices)</li>
    <li>Client Computer (to make sure all permissions and attributes are working correctly)</li>
  </ul>
  <h4>Notes and Observations:</h4>
    <p>
  In the lab we used Active Directory to create organizational units. We made a MAIN OU to hold all the other OUs which we named Marketing, HR, and Accounting. In these three OUs we had to have a total of five user accounts. In Accounting we had Kevin Malone and Oscar Martinez. In HR we had Toby Flenderson, and in Marketing we had Jim Halpert and Dwight Schrute. After we had created our five users we then had to develop a group structure. We decided to great a global group for each OU inside the MAIN and named them GGAccounting, GGHR, and GGMarketing. Along with theses global groups we also created a domain local group for each OU named DLAccounting, DLHR, and DLMarketing. We gave full permissions for each global group to the matching domain local. From their the domain locals were all given permission to access top level folder titled Flat Earth Documents. With that folder we had the folders Flat Earth Accounting, Flat Earth HR, and Flat Earth Marketing. We gave each domain local group access to their matching folder and to test the permissions we also go DLAccounting access to Flat Earth Marketing. The test was successful and users in Accounting could access the folder but those in Marketing still did not have access to Flat Earth Accounting. For the test we used user KMalone (Kevin Malone). After we had tested the users we were then asked to add a printer to the network by using network-attached printer sharing. Along with this we also had to decide who had access to this printer. We decided upon Accounting having printer access due to us already being signed into an Accounting user. Here is the sheet that confirmed the connection worked <a href="https://github.com/DesignsMP/Lab_Reports/blob/master/Permissions%20and%20Attributes/Printed%20Sheet.md"> Printer Confirmation<a/>
    </p>
  <h4>Diagrams, flowcharts, and figures:</h4>
  I did draw out a diagram to show the hierarchy of the MAIN OU along with the Folder locations.
 
 ![Lab 4 Diagram](https://user-images.githubusercontent.com/31741807/54775264-9e768800-4bdb-11e9-98e6-e04c58afc072.png)

  <h4>References:</h4>
    References were both given in class and found online. This includes;
    <ul>
      <li> Names of computers and accounts</li>
      <li> IP Addresses</li>
      <li> Product Keys</li>
      <li> Passwords</li>
    </ul>
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li>How do you deny individual people certain permissions without denying everyone that permission?</li>
  <li></li>
  <li></li>
  <li></li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
    <p>
   In Conclusion 
    </p>
