<h1>Domain Controller & Distributed File System</h1>
  <h4>Objectives:</h4>
  <p>Our objective for this lab was to create a second domain controller for our domain and to replicate using the Distributed File system (DFS).
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
    To begin this lab we had to review our notes from lab 3 in order to remember how to set up a virtual server. The server we had been using was named WinServer3B so for this lab we would be setting up WinServer3A. Using powershell we enabled remote desktop by using the commands "Enable-PSRemoting" and "Enable-WSManCredSSP". Next we changed the IP Address that it was given by default. Using the control panel we went to the network connections tab -> Right clicked the Ethernet network -> went to IPv4 Properties and from there we changed the IP address along with the preferred and alternate DNS server. After that we went to change the name of the server. To do this we went back to the control panel and typed in system -> clicked change computer name -> and chose the join domain option using the user Jim Halpert from Marketing. We did encounter an issue when trying to remote desktop into the server the first time, we were accidently using "/" instead of "\" when selecting the user. Once this was done we used the server manager to install active directory with the same settings we used for WinServer3B. We added the domain controller services but we did not need the DNS but instead added global. Once the server was up and running we had to promote it to a domain controller. We then created a folder on WinServer3A's desktop. Then using the advanced sharing option under the folder we made the sharing permissions full control. Next we went to the security tab, removed the default users, and added the Domain Local groups in our domain, along with applying any necessary restrictions. After that is was time to use the DFS. We opened up the server manager again and 
<ol>
      <li> selected roles and features </li>
      <li> under the file and storage tab we selected both DFS options </li>
      <li> under tools we selected the DFS Management option </li>
      <li> we then created a name space on both servers titled "UserData" </li>
      <li> created a path to the WinServer3B\UserData namespace </li>
      <li> and we finally ran into a problem </li> 
</ol> 
We could not connect the servers together due to the fact that both had a namespace titled "UserData". To fix this problem we simply deleted the namespace on WinServer3A which allowed WinServer3B to make the connection. Next came the stage to replicate the folders by <ol>
  <li>first selecting Multi-purpose Replication Group </li>
  <li> then selected the name "Company Files" </li>
  <li> and selected a full mesh and continuous replication </li>
</ol>
  This is where we encountered our second and crippling problem. When we went to select which servers files to replicate there were not any servers displayed to select. After doing some searching we found that the servers had automatically replicated the files for us and was not allowing us to do it again. This also meant that while it was replicating the information, due to it being automatic we could not adjust the replication settings in any way which means we could not prevent or restrict which files would be replicated. We believe this was due to the fact that we were setting both servers up for replication at the same time and, seeing the "UserData" path, the computer decided to replicate the files for us.
  <br> The advantages you get with using DFS are administrators being apply to simplify access to multiple shared-file resources, eliminates the need for users to browses the network for resources, and makes files appear to be in a single hierarchical structure.
  <br> Having a domain-based namespace has some benefits compared to a standalone namespace such as easy replication, a built in fault tolerance, and the load balancing feature which means that files would be pulled from multiple locations to speed up the download process.
  <br> The purpose of the referral server is allow direct access to shared folders using its real location . It is highly recommended to have a back-up referral server because if one server were to go down, the second server would be promoted to the primary and would still allow real location access to the shared folders.
    </p>
  <h4>Diagrams, flowcharts, and figures:</h4>
  There were no diagrams or figures with this lab but we did take snip clips of each stage in which we had to select something.
  <br>
 ![unnamed](https://user-images.githubusercontent.com/31741807/55181047-cc6a4800-5158-11e9-960f-cca8d458aeab.png)

 ![unnamed (1)](https://user-images.githubusercontent.com/31741807/55180015-ae034d00-5156-11e9-804f-4f3dfb5db568.png)
 ![unnamed (2)](https://user-images.githubusercontent.com/31741807/55180018-af347a00-5156-11e9-8ca7-7443710caf14.png)

  <h4>References:</h4>
    References were both given in class and found online. This includes;
    <ul>
      <li> Names of computers and accounts</li>
      <li> IP Addresses</li>
      <li> Product Keys</li>
      <li> Passwords</li>
      <li><a href="https://nedimmehic.org/2017/10/05/how-to-install-and-configure-distributed-file-system-dfs-2016-part-1/">Tutorial Part 1</li>
      <li><a href="https://nedimmehic.org/2017/11/01/how-to-install-and-configure-distributed-file-system-dfs-2016-part-2/">Tutorial Part 2</li>
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
