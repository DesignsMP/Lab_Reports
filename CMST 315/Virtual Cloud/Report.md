<h1>Virtual Cloud</h1>
  <h4>Objectives:</h4>
  <p>Our objective for this lab was to use Microsoft Azure to create a Linux or Windows cloud web-server.
</p>
  <h4>Materials</h4> 
  <ul>
    <li>Pencil (to write down notes)</li>
    <li>Paper (to store notes)</li>
    <li>Remote Desktop (to communicate with rack server without having  to access it directly)</li>
    <li>Microsoft Azure (to create, configure, and run cloud-based virtual machines)
    <li>Bash ( to download, update, and edit the virtual machines/ web-server)
    <li>Computers (to access applications such as Microsoft Azure)
  </ul>
  <h4>Notes and Observations:</h4>
    <p>
      For this lab we were to set up a web-server using cloud services offered by Microsoft Azure. We had the choice of creating a Windows or Linux web-server. Due to having never worked with the Linux OS before my group decided to create a Linux server. Using the Microsoft Azure tutorial we first created a virtual machine named "myVM" which each person created their own. We then created a group to store all of our resources which we named "myResourceGroupVM" based on the tutorial. We later created another virtual machine due to the tutorial mentioning it named "myResourceGroupDisk" which we later found out was not necessary to get the web-server running. Using bash we connected the VM with ssh using the public IP address Microsoft provided us. Next was defining the size of the VM which I struggled with at first. I wanted the VM to have a larger disk space due to thinking more is better, I later find out that since the size I chose used four cores I could not use it for this lab. With the free trial version of Azure the user is only allowed a maximum of four cores. I was using all four cores for the VM and I had not created my disk yet which required a minimum of two cores. I decided to down size to a size that only used two cores and was still bigger than the original size of my VM. This allowed the disks two cores to work and reaching my limit of four cores. From here I started the virtual machine for which I did not stop until after the lab was over. Once the VM and Disk were created they needed to be attached. Through bash I was able to attach the disk with no trouble and then partitioned the disk due to their suggestion to do so. From here we skipped to step fifteen which is the step that adds the apps and javascript to get the server up and running. We could to use the MEAN stack (MongoDB, Express, AngularJS, Node.js) due to having worked with three of the four apps in past projects. First we installed the apps in the order of Node.js, MongoDB, Express, and finally AngularJS. Node.js allowed for us to install any packages we needed to run the apps. MongoDB then created a server with a database to store information entered on the page. Express would then create the routes to the server, that way the local computer could access the files. Finally came AngularJS which was needed for the user to access the created routes else there was no point to the routes. All of the javascript used for this lab, along with the index.html page, was provided by Microsoft and did not require any editing to serve our purposes. Using the command node.js server.js the web-server was up and running. An issue I had run into was, although the web-server was running I could not access the page itself using port 3300. A classmate later showed me how to add another port to my VM by going to the Networking tab under settings and then clicked "Add inbound port rule" where I chose to use port 3300 which is the port selected by default for the tutorial.
    </p>
    <ol>
     <li>
        Advantages:
            <ul>
              <li> Scalability: cloud infrastructure size is based on the businesses needs</li>
              <li> Tools: when using the cloud most services offer built-in tools that can help acheive the companies needs</li>
            </ul>
        Disadvantages:
            <ul>
              <li> Downtime: it may take awhile to get a cloud server back up and running</li>
              <li> Vulnerability: due to being solely on the web cloud services have a higher vulnerability to cyber attacks</li>
            </ul>
     </li>      
     <li> Businesses need to consider which cloud service provider they want to go with whether that be Microsoft Azure, Google Cloud Services, and AWS. Another thing to consider is disaster recovery, if the devices containing their cloud services were to be damaged or lose power there has to be a back-up plan or risk losing all of the information that had been stored in the cloud. These are a few things to think of before they switch IT to the cloud.</li>
     <li> Examples of built-in Azure configurations and services include:
          <ul>
            <li> Migration guides</li>
            <li> Azure media player</li>
            <li> Visual Studio Code integration</li>
          </ul>
     </li>
    </ol>
  <h4>Diagrams, flowcharts, and figures:</h4>
  Here is an image to demonstrate how I got the web-server up and running.
  <br><br><br>
  
  ![Capture](https://user-images.githubusercontent.com/31741807/56990432-aa4e5600-6b5a-11e9-9356-530b8ede58b9.PNG)

  <h4>References:</h4>
    References could be found online with these links;
    <ul>
      <li><a href="https://portal.azure.com/#home">Microsoft Azure</li>
      <li><a href="https://docs.microsoft.com/en-us/azure/virtual-machines/linux/">Linux Tutorial</li>
    </ul>
  <h4>Questions:</h4>
  A few things I am still confused on are:
  <ol>
  <li> Who was the first to implement a cloud based server?</li>
  <li> Would the cloud work well for something like a video game  server?</li>
  <li> Does Apple have any iOS cloud servers?</li>
  <li> Can a cloud server contain cloud servers?</li>
  </ol>
  <h4>Conclusion and Reflection:</h4>
    <p>
    In conclusion I now understand the importants on how Cloud services can greatly benefit a company, but risks should still be assessed at all times. One of the major reasons why most businesses do not go with a cloud server to store their information is cost. It can get really expensive to use a service, like Microsoft Azure, for all of the companies files and applications. Plus the more virtual machines used the fast the data will get used up. For the lab we used a free account with our student status which gave us a $200.00 credit limit. By the end of the lab I was a little of $100.00 but I lost most of my credit when I accidentally had two virtual machines running at the same time. If a company can look past the price tag and truly believe that they would make more money being on the cloud, then a cloud-based company server would provide numerous advantages over those who do not implement cloud technology.
    </p>
