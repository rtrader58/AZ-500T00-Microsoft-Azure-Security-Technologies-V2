# AZ-500T00 All Learning Paths Errata


Updated March 2024 <br>
When starting each lab choose Yes when prompted to be visible in networks<br>

# Learning Path 1 Manage Identity and Access - Total lab time ~150 Minutes (3.5 hour)

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 1 – Role-Based Access Control ~30 Minutes (90 Min)

### Exercise 2 – Create a Junior Admins group containing the user account Isabel Garcia as its member

Task 1: <br>
Step 1:  PowerShell is now called Windows Terminal (Admin) when right clicking on the start menu.<br>
Step 2:  When copying and pasting command it sometimes pastes wrong, 
Ensure the command is Install-Module <br>

### Exercise 3 – Creating a Service Desk Group; containing the user account Dylan Williams as its member

Task 1: Use Azure CLI to create a user account Dylan Williams<br> 
If you encounter an error during this lab that indicates the clock is out of sync or the current time is in error, use the Settings app in the VM to synchronize the computer’s clock and then retry the step<br>
Wait for step 1 to complete before moving on to step 2 <br>
After running step 3 choose Edge Browser and enter your Azure tenant admin account and password <br>

# Learning Path 2 – Implement Platform Protection ~135 Minutes (180)

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 02 – Network Security Groups and Application Security Groups ~45 Minutes (60 Min) 

### Exercise 1:  Filter network traffic with a network security group using the Azure portal

Task 1:  Create a virtual network <br>
Before step 1:  Logon into the Azure portal with your global administrator account<br>
Step 2: You may have to search for Virtual network, if you have to search then click Create <br>

Task 3: Create a network security group<br>
Step 2: You may have to search for Network security group, if you have to search then click Create - ensure you choose Network Security Group (Not network security group classic) <br>
After step 10 - Create the required Vnet using the following steps <br>
Search for Virtual network <br>
Click Create <br>
Use the provided Resource Group <br>
Nme the Vnet:  AZ500LAB09-vnet <br>
Select Review+Create, then Create <br>

Task 4: Create inbound NSG security rules to all traffic to web servers and RDP to the servers.<br>
Note -- when creating the rules leave the source as "Any"<br>

Task 6: Create virtual machines<br>
Step 2:  Choose Windows Server 2019 Datacenter<br>
Step 5:  Select Disable not off<br>
Task 8: Associate network interfaces to an ASG<br>
Step2:  Select Application security group, then select Configur the application security group<br>

Task 9:  Test traffic filters <br>
Step 6:  When pasting from the lab instructions the syntax is wrong. <br> 
	It pastes  <br>
		mstsc /v;myVmWeb <br>
	It should be   <br>
		mstsc /v:MyVmWeb <br>

## Lab 03 – Azure Firewall ~45 Minutes (60 Min) 

### Exercise 1:  Deploy and test an Azure Firewall 

Task 1:  Deploy the Azure firewall 
Step 1:  When prompted:  Logon into the Azure portal with your global administrator account.  <br>
Step 3:  Select radial button under Firewall management - Use Firewall rules (classic) to manage this firewall<br>
Step 3:  Select Test-FW-VN from the Virtual network dropdown<br>

Task 2:  Create a default route <br>
Step 2:  Click +Create<br>
Step 5:   Search for Route Tables and select <br>

## Lab 7 – Configuring and Securing ACR and AKS ~45 Minutes (60 Min)

If the creation of the storage account fails, click on Show Advanced Settings and manually create a storage account.  Ensure you choose East US. <br>

### Exercise 1:  Configuring and Securing ACR and AKS

Task 1:  Create an Azure Container Registry <br>
Step 1:  When prompted:  Logon into the Azure portal with your global administrator account. <br>

Task 3: Create an Azure Kubernetes Service cluster<br>
Step 6:  Do not continue until the cluster is complete<br>After Step 10 create a Vnet using the following Steps<br>
Search for Virtual networks - Select Virtual Networks <br>
Select Create <br>
On the Basics tab <br>
Choose the Resource Group created peviously in the lab <br>
Nme the Virtual network:  AZ500LAB09-vnet <br>
Click review+create then Create <br>

Task 4:  Give AKS permissions to access the ACR <br>
Step 2:   Look in your resources group to see the name of the container registry, replace <ACRuniquename> with the container name <br>

Task 5: Deploy an external service to AKS<br>
Step 5: There no ellipses. Move your cursor to the upper right hand corner on the editor and left click you will see the option to save and also option to close.<br>

# Learning Path 2 Additional Labs ~240 Minutes (360 Min)

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Nmae change)

## Lab 102 – VNet Peering ~45 Minutes (60 Min) 

### Exercise 1:  Create Virtual Networks and implement Peering

Task 1:  Create virtual networks <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
Step 3:  You may have to search for Virtual network, if you do click Create<br>
Step 3:  Select Default subnet and change name to Subnet1 <br>
Step 4:  You may have to search for Virtual network, if you do click Create<br>
Step 4:  Select Default subnet and change name to Subnet2 <br>

Task 2:  Peer virtual networks <br>
Step 3:  <br>
		This virtual network<br>
		Peering Link name:  myVirtualNetwork1-myVirtualNetwork2<br>
		Remote virtual network<br>
		Peering link name:  myVirtualNetwork2-myVirtualNetwork1<br>
		Leave the remaining settings as default <br>

Task 3:  Peer virtual networks <br>
Step 5:   Select Disable for Boot Diagnostics when creating both VMs <br>
Task 4:  Communicate between VMs <br>
Step 7:   Does not paste correctly – change the ; to a : <br>
Step 10: Disregard <br>

## Lab 103 – NVA ~75 Minutes (60 Min)

### Exercise 1:  Create a route table 

Task 1:  Route network traffic with a route table using the Azure Portal <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
If Route Tables does not show up as an option Search for it <br>

Task 5: Associate myRouteTablePublic to your Public subnet <br>
Step 2:  If you get an error the Subnet Address Range cannot be blank.  Populate it with the IP Adress ffrom Task 3 > Step 2 > Public IP Addresss range provided in the box <br>

Task 6:  Create an NVA <br>
Step 8:  Select - “Enable with custom storage Account” <br>
Use the name that auto populates <br>

Task 11:  Turn on IP forwarding with myVmNva <br>
Step 4:   Does not paste correctly – change the ; to a : <br>

## Lab 104 – Azure Bastion ~30 Minutes (60 Min)

### Exercise 1:  Implement Azure Bastion

Task 1:  Enable Azure Bastion on your subscription <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
If the creation of the storage account fails, click on Show Advanced Settings and manually create a storage account.  Ensure you choose East US. <br>
Step 4:  When running the second PowerShell command remove the word “undefined” at the end of the command <br>
Step 8:  Select Save not OK<br>

Task 2:  Create a Bastion host <br>
Step 5:  The virtual network / subnet may take up to 10 minutes before it shows up in the drop down <br>

Task 3: Connect to a VM using a bastion host<br>
Step 3:  Make sure you clear the check box "Open in a new window"<br>

## Lab 105 – VM Secure Admin Access ~40 Minutes (60 Min)

Task 1:  Create SSH keys with PuTTygen <br>
Before step 1:  Logon into the Azure portal with your global administrator account.  <br>
Step 1:  After pasting URL remove “/undefined” from end <br>

## Lab 106 – Azure Disk Encryption ~20 Minutes (60 Min)

Task 3: Encrypt the virtual machine<br>
Step 2: You cannot configure the disk to be unencrypted, so the corresponding output will not show the same thing that the lab step shows you. This is expected, continue on.<br>

## Lab 107 – VM Update Management ~40 Minutes (60 Min) 

### Exercise 1:  Use Azure Automation to manage Windows Updates

Task 1:  Enable Update Management <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
Step 3:  Under Operations click on Guest + host updates <br>
Click on “Go to Update management <br>

Task 5:  Configure Alerts <br>
Step 7:  No longer required<br>

# Learning Path 3 - Secure Data and Applications ~150 Minutes (180 Min)

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 8 – Securing Azure SQL Database ~20 Minutes (60 Min)

Task 2:  Configure Advanced Data Protection <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
Step 2:  On the server blade, in the Security section, click Microsoft Defender for Cloud. <br>
Step 5:  In the Azure Defender for SQL: Enabled at the subscription-level (Configure) parameter, click (configure).<br>
Step 7:  Back to Microsoft Defender for Cloud blade, review Recommendations and Security incidents and alerts. <br>

Task 4 : Configure auditing<br>
Step 3:  Click on Server Settings then set the Auditing switch to ON to enable auditing.<br>

## Lab 9 – Securing Azure Storage ~55 Minutes (60 Min)

### Exercise 1: Service endpoints and security storage

Task 1:  Create a virtual network <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
Step 2:  You may have to search for Virtual Network<br>
Step 3:  Leave default security settings (this will choose basic DDOS) <br>

Task 4:  Restrict network access to a resource <br>
Steps do not work as written, do the following: <br>
Select the navigation pane in the Azure portal <br>
Select Storage Account <br>
Click on New <br>
Fill out the form with the information from the lab <br>

Task 5:  Create a file share in the storage account<br>
Step 2:  File share is now called File service.  You may have to scroll on the Overview tab to see the link to File service.  The graphic in the lab does not match the interface. <br>

Task 6: Restrict network access to a subnet<br>
Step 1:  Under Security + networking for your storage account select networking<br>
Step 5:  Click Add, then click Save<br>
Step 6:  Under Security + networking for your storage account select Access keys<br>
Step 7:  Copy the Key and connection string to notepad<br>

Task 8: Confirm access to storage account <br>
Step 6: In the third command replace storage-account-name with the name of your storage account leave the rest of the string <br>

Task 9: Confirm access is denied to storage account<br>
Step 3:  Repeat steps 1-6 of Task 8<br>

## Lab 10 – Key Vault (Implementing Secure Data by setting up Always Encrypted) ~75 Minutes (60 Min)

## Exercise 2: Key Vault

Task 1: Create and configure a Key Vault
Step 11:  in the resources pane of the resource group, select the keyvault you just created 

## Exercise 3: Configure an Azure SQL database and a data-driven application

Task 2: Create a policy allowing the application access to the Key Vault<br>
Step 3:  Replace  ‘<Azure_AD_Application_Id>’ with your AP ID recorded in earlier step.  Make sure to include the ‘ at the beginning and end<br>

Task 5: Create a table in the SQL Database and select data columns for encryption <br>
Step 10:  If you get an error when connecting, manually type in your password <br>

Step 14:  If the paste does not paste correctly, open notepad on the Lab VM not the RDP session and paste the query into notepad.  Copy and paste from notepad into the the RDP session <br>
	
# Learning Path 4 – Manage Security Operations - Lab 11, 12 and 13 launch in a single lab environment – Total time ~135 hours (90 Min)

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 11 – Azure Monitor ~30 Minutes

Task 3: Enable the Log Analytics virtual machine extension <br>
Step 1: Before beginning this task, ensure that the Log Analytics Workspace deployment has completed successfully, it should take 1-2 minutes<br>
Step 2 – if the VM is not listed, wait a few minutes and then refresh the view. It can take up to 15 minutes for the VM to appear in the list. Also, verify that the VM you created in Task 1 is Running.<br>
Step 4 - 5: It can take a few minutes to connect.  (On 11/5/2021 this took 2.5 minutes) This is a great time to stretch & hydrate!<br>

Task 5: View and query collected data<br>
Step 3: Close the video in the details section of this page, and ignore the instruction to click “get started”<br>
Step 4: Navigate to the Virtual Machines queries in the All Queries column or use Search<br>
Step 5: It doesn’t matter which queries you run, this task is to show you VM log data being gathered. Note that some queries will have no results as not enough data has been gathered yet.<br>

# ***** DO NOT END THE LAB!!  After completing Lab 13 use the drop down window at the top to move to lab 14  DO NOT END THE LAB!! *****

## Lab 12 – Security Center ~60 Minutes

Task 1: Configure Security Center <br>
Step 1: You’re already logged in, you can skip this step<br>
Step 2: Brand name change occurred. Security Center is called Microsoft Defender for Cloud now<br>
Step 3: If you see both the subscription and the new instance that you created in Lab 13, select both of them. <br>
Also Step 3: After confirmation, click Install Agents<br>
Step 4: Click the Overview blade, and then in the details pane click Enable Azure Defender<br>
Step 7:  On the Settings blade verify that Log Analytics agent for Azure VMs is On if off turn on<br>
Step 8:  Is on the pop up when you turn on the Log Analytics<br>
The steps return to normal at #10. Steps 2-10 are a bit of a mess.<br>
Step 10: In the Management section, click the Workflow Automation blade<br>
Step 13: JFYI you can’t create a workflow automation yet because you don’t have any Logic Apps yet. You’ll create those in the next lab.<br>
Steps 14 & 15: Skip<br>

Task 2: Implement the Security Center recommendation <br>
Step 2: in the Cloud Security section, there may not be a score yet.  It can take up to 60 minutes to evaluate. Just continue with the lab.<br>
Step 3: Click the Inventory tile<br>

Task 3: Implement the Security Center recommendation to enable Just in time VM Access<br>
Replace steps 1 and 2 with:<br>
Open the Virtual Machines space<br>
Select the VM you created earlier<br>
In the Settings section, click the Security blade<br>
Click the Explore just-in-time access in Defender for Cloud<br>
If JIT does not appear as an option within 30 minutes, move on to Lab 15.<br> It is not necessary to complete the JIT VM Access task to complete the labs.<br>

# ***** DO NOT END THE LAB!!  After completing Lab 14 use the drop-down window at the top to move to lab 15.  Do not end the lab!! *****<br>

## Lab 13: Azure Sentinel ~45 Minutes

Task 2: Configure Azure Sentinel to use the Azure Activity data connector<br>
Step 10:  Per the note it may take anywhere from 10-30 minutes before the connector shows Connected. Please wait for it to show Connected before proceeding.<br>

Task 4: Create a playbook<br>
Steps 1-3: Do these tasks in the VM, not your local OS.<br>

Task 5: Create a custom alert and configure a playbook as an automated response<br>
Step 10: Under Alert automation, select the drop-down and check the Select all box<br>

Task 6: Invoke an incident and review the associated actions<br>
For Steps 1-3, disable JIT VM access for myVM using the steps in Lab 14 Task 3<br>
Step 5: This can take several minutes to show up. Stretch & hydrate!<br>
