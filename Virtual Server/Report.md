<h1>Virtual Windows Server</h1>
  <h4>Objectives:</h4>
    The objective for this lab was to understand virtual machines and servers and how they allow you to run several different machines all on one computer or server. With the possibility it also allows people to have multiple machines each with the ability to be customized to a specific need without affecting any of the other virtual machines.
  <h4>Equipment List:</h4>
  <ul>
    <li>Pencil (to write down notes)</li>
    <li>Paper (to store notes)</li>
    <li>Hyper-V (to manage all of our virtual machines)</li>
    <li>Dell rack server (to store and run all of our virtual machines)</li>
    <li>Windows Server 2016 (the purpose of the virtual server and tool for the next lab)</li>
    <li>Remote Desktop (to communicate with rack server without having  to access it directly)</li>
  </ul>
  <h4>Notes and Observations:</h4>
    <p>
    In order to start this project we had to configure a rack server in order to store any virtual machines. We probably could have used a normal computer but the lab computers would erase any changes we made. In the configuration we set RAID from level 1 to level 0 in order to use all of the available disk space rather than mirroring. After that we deleted all partitions currently on the drive. Instructor used our lab as a test for using remote desktop, which was done outside of class. I do not fully understand how to enable remote desktop. After that we installed Hyper-V, while installing we used the username Hyper3\Administrator. We then accessed powershell in order to enable PSRemoting and WSMANCredSSP. This was used to create firewall rules for our domain and to allow us to securely use our credentials over the network. Then we assigned an ethernet port along with making changes to network manager and group policies. After all that was in order we pinged the server to see if we could make a connection from a remote desktop. Which we were able to on the first try this time.
    </p>
  <h4>Diagrams, flowcharts, and figures:</h4>
  There were no diagrams or figures with this lab.
  <ul>
    
  </ul>
  <h4>References:</h4>
    References were both given in class and found online. This includes;
    <ul>
      <li> Names for the computers and accounts</li>
      <li> IP address information</li>
      <li> Product keys</li>
      <li> Passwords</li>
  <li><a href="https://timothygruber.com/hyper-v-2/remotely-managing-hyper-v-server-in-a-workgroup-or-non-domain/">Remote Hyper V</a></li>
  <li><a href="https://www.petri.com/using-syspre-windows-10"> Syspre</a></li>
   <li><a href="https://www.nakivo.com/blog/creating-configuring-vms-in-windows-server-2016-hyper-v/">Configure VM's</a></li>
    </ul>
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> How did people come up with the idea of virtual machines?</li>
  <li> How many virual machines are commonly used in a business?</li>
  <li> What all can one do with a server?</li>
  <li> What are all the different things you can do with remote desktop?</li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
  
