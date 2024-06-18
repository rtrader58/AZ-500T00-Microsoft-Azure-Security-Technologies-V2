# AZ-500T00 Learning Path 2 Labs Errata

When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

# Learning Path 2 – Implement Platform Protection ~95 Minutes (120)

## Lab 02 – Network Security Groups and Application Security Groups ~45 Minutes (60 Min) 

### Exercise 1:  Filter network traffic with a network security group using the Azure portal

Task 1:  Create a virtual network <br>
Step 4:  The Resource Group has already been created, select it from the dropdown menu <br>

Task 2: Create application security groups <br>
Step 3:  The Resource Group has already been created, select it from the dropdown menu <br>

Task 3: Create a network security group<br>
Step 3:  The Resource Group has already been created, select it from the dropdown menu <br>

### Exercise 2: Deploy virtual machines and test network filters

Task 1: Create a virtual machine to use as a web server <br>
Step 3:  The Resource Group has already been created, select it from the dropdown menu <br>
Step 3:  Choose Windows Server 2019 Datacenter - x64 Gen 2<br>
Step 3:  Use the Labuser password in the Resources tab, if the password is not long enough add additional characters <br>

Task 2: Create a virtual machine to use as a web server <br>
Step 2:  The Resource Group has already been created, select it from the dropdown menu <br>
Step 2:  Choose Windows Server 2019 Datacenter - x64 Gen 2<br>
Step 2:  Use the Labuser password in the Resources tab, if the password is not long enough add additional characters <br>

Task 3: Associate each virtual machines network interface to its application security group <br>
Step 3:  On the myVMWeb blade, in the Networking section, click the Application security groups <br>
Step 4:  Click + Add application security groups, in the Application security group list, select myAsgWebServers, and then click Add <br>
Step 6:  On the myVMWeb blade, in the Networking section, click the Application security groups <br>
Step 7:  Click + Add application security groups, in the Application security group list, select myAsgMgmtServers, and then click Add <br>
Note - if you want to verify the NSG and ASG attempt to RDP into the myVmWeb server and attempt to connect to the default web site on the myVMMgmt server -  both attepts should fail <br>


## Lab 3 – Azure Firewall ~45 Minutes (60 Min) 

### Exercise 1:  Deploy and test an Azure Firewall 

Task 1:  Deploy the Azure firewall 
Step 1:  When prompted:  Logon into the Azure portal with your global administrator account.  <br>
Step 3:  Select radial button under Firewall management - Use Firewall rules (classic) to manage this firewall<br>
Step 3:  Select Test-FW-VN from the Virtual network dropdown<br>

Task 2:  Create a default route <br>
Step 2:  Click +Create<br>
Step 5:   Search for Route Tables and select <br>
