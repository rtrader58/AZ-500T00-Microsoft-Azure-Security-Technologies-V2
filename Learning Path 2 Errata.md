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

### Clean up resources

Replace step 1 with the following: <br>

Step 1:  Open the Cloud Shell by clicking the first icon in the top right of the search area in the Azure portal > Select PowerShell > click Mount Storage Account > in the drop down choose your subscription > click Apply > select We will create a storage account for you > click next <br>

## Lab 3 – Azure Firewall ~45 Minutes (60 Min) 

### Exercise 1:  Deploy and test an Azure Firewall 

Task 1:  Use a template to deploy the lab environment <br> 
Step 4:  The allfiles folder is located on the desktop not in the F drive <br>
Step 6:  Create a password of at least 12 characters, recommendation using the password in the Resources tab add additional characters to make it at least 12, paste it into Notepad for later use <BR>

Task 2:  Deploy the Azure firewall <br>
Step 4:  Click Next : Tags > Click Review + create and then click Create.

Task 4:  Configure an application rule <br>
Step 5:  Before continueing wait for the rule to finish configuring before moving on <br>

Task 5:  Configure a network rule <br>
Step 5:  Before continueing wait for the rule to finish configuring before moving on <br>

Task 6:  Configure the virtual machine DNS servers <br>
Step 3:  On the Srv-Work blade, in the Networking section, click Networking Settings <br>

Task 7: Test the firewall <br>
Step 9:  Select do not use recommended setting as if will block the results of the test <br>

### Clean up resources

Replace step 1 with the following: <br>

Step 1:  Open the Cloud Shell by clicking the first icon in the top right of the search area in the Azure portal > Select PowerShell > click Mount Storage Account > in the drop down choose your subscription > click Apply > select We will create a storage account for you > click next <br>
