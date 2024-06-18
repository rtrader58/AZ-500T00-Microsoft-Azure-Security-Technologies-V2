# AZ-500T00 All Learning Paths Errata

Updated June 2024 <br>
When starting each lab choose Yes when prompted to be visible in networks<br>
# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)
 
# Learning Path 1 Manage Identity and Access - Total lab time ~30 Minutes (90)

## Lab 1 – Role-Based Access Control ~30 Minutes (90)

### Exercise 1: Create the Senior Admins group with the user account Joseph Price as its member

Task 2: Use the Azure portal to create a Senior Admins group and add the user account of Joseph Price to the group <br>
Step 4 and 5: Click the T to paste the Joseph account into the Search bar then select the displayed account <br>

### Exercise 2 – Create a Junior Admins group containing the user account Isabel Garcia as its member

Task 1:  Use PowerShell to create a user account for Isabel Garcia <br>
Step 1:  Select PowerShell > click Mount Storage Account > in the drop down choose your subscription > click Apply > select We will create a storage account for you > click next <br>

### Exercise 3 – Creating a Service Desk Group; containing the user account Dylan Williams as its member

Task 1: Use Azure CLI to create a user account Dylan Williams<br> 
If you encounter an error during this lab that indicates the clock is out of sync or the current time is in error, use the Settings app in the VM to synchronize the computer’s clock and then retry the step<br>

# Learning Path 2 – Implement Platform Protection ~95 Minutes (120)

## Lab 02 – Network Security Groups and Application Security Groups ~45 Minutes (60 Min) 

### Exercise 1:  Filter network traffic with a network security group using the Azure portal

Task 1:  Create a virtual network <br>
Before step 1:  Logon into the Azure portal with your global administrator account<br>
Step 2: You may have to search for Virtual network, if you have to search then click Create <br>

Task 3: Create a network security group<br>
Step 2: You may have to search for Network security group, if you have to search then click Create - ensure you choose Network Security Group (Not network security group classic)<br>

Task 4: Create inbound NSG security rules to all traffic to web servers and RDP to the servers. <br>

Note -- when creating the rules leave the source as "Any" <br>

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

## Lab 3 – Azure Firewall ~45 Minutes (60 Min) 

### Exercise 1:  Deploy and test an Azure Firewall 

Task 1:  Deploy the Azure firewall 
Step 1:  When prompted:  Logon into the Azure portal with your global administrator account.  <br>
Step 3:  Select radial button under Firewall management - Use Firewall rules (classic) to manage this firewall<br>
Step 3:  Select Test-FW-VN from the Virtual network dropdown<br>

Task 2:  Create a default route <br>
Step 2:  Click +Create<br>
Step 5:   Search for Route Tables and select <br>

# Learning Path 3 - Secure Data and Applications ~140 Minutes (180 Min)

## Lab 4 – Configuring and Securing ACR and AKS ~45 Minutes (60 Min)

If the creation of the storage account fails, click on Show Advanced Settings and manually create a storage account.  Ensure you choose East US. <br>

### Exercise 1:  Configuring and Securing ACR and AKS

Task 1:  Create an Azure Container Registry <br>
Step 1:  When prompted:  Logon into the Azure portal with your global administrator account. <br>

Task 3: Create an Azure Kubernetes Service cluster<br>
Step 6:  Do not continue until the cluster is complete<br>
After step 10 - Create the required Vnet using the following steps <br>
Search for Virtual network <br>
Click Create <br>
Use the provided Resource Group <br>
Nme the Vnet:  AZ500LAB09-vnet <br>
Select Review+Create, then Create <br>

Task 4:  Give AKS permissions to access the ACR <br>
Step 2:   Look in your resources group to see the name of the container registry, replace <ACRuniquename> with the container name <br>

Task 5: Deploy an external service to AKS<br>
Step 5: There no ellipses. Move your cursor to the upper right hand corner o the editor and left click you will see the option to save and also option to close.<br>

## Lab 5 – Securing Azure SQL Database ~20 Minutes (60 Min)

Task 2:  Configure Advanced Data Protection <br>
Before step 1:  Logon into the Azure portal with your global administrator account. <br>
Step 2:  On the server blade, in the Security section, click Microsoft Defender for Cloud. <br>
Step 5:  In the Azure Defender for SQL: Enabled at the subscription-level (Configure) parameter, click (configure).<br>
Step 7:  Back to Microsoft Defender for Cloud blade, review Recommendations and Security incidents and alerts. <br>

Task 4 : Configure auditing<br>
Step 3:  Click on Server Settings then set the Auditing switch to ON to enable auditing.<br>

## Lab 6 – Service Endpoints and Securing Storage ~75 Minutes (60 Min)

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
	
# Learning Path 4 – Manage Security Operations – Total time ~210 Minutes 

## Lab 7 – Key Vault ~75 Minutes (60)

## Exercise 2: Configure the Key Vault resource with a key and a secret

Task 1: Create and configure a Key Vault
Step 11:  in the resources pane of the resource group, select the keyvault you just created 

## Exercise 3: Configure an Azure SQL database and a data-driven application

Task 2: Create a policy allowing the application access to the Key Vault<br>
Step 3:  Replace  ‘<Azure_AD_Application_Id>’ with your AP ID recorded in earlier step.  Make sure to include the ‘ at the beginning and end<br>

Task 5: Create a table in the SQL Database and select data columns for encryption
Step 10:  If you get an error when connecting, manually type in your password

Step 14:  If the paste does not paste correctly, open notepad on the Lab VM not the RDP session and paste the query into notepad.  Copy and paste from notepad into the the RDP session

# NOTE - Labs 8, 9 and 10 launch in a single lab environment - Do Note End between labs ~150 Minutes (120)
### Keep an eye on the lab timer.  You will need to extend the lab at least once to complete 

## Lab 8 – Azure Monitor

Task 3: Enable the Log Analytics virtual machine extension <br>
Step 1: Before beginning this task, ensure that the Log Analytics Workspace deployment has completed successfully, it should take 1-2 minutes<br>
Step 2 – if the VM is not listed, wait a few minutes and then refresh the view. It can take up to 15 minutes for the VM to appear in the list. Also, verify that the VM you created in Task 1 is Running.<br>
Step 4 - 5: It can take a few minutes to connect.  (On 11/5/2021 this took 2.5 minutes) This is a great time to stretch & hydrate!<br>

Task 5: View and query collected data<br>
Step 3: Close the video in the details section of this page, and ignore the instruction to click “get started”<br>
Step 4: Navigate to the Virtual Machines queries in the All Queries column or use Search<br>
Step 5: It doesn’t matter which queries you run, this task is to show you VM log data being gathered. Note that some queries will have no results as not enough data has been gathered yet.<br>

# ***** DO NOT END THE LAB!!  After completing Lab 8 use the drop down window at the top to move to lab 9  DO NOT END THE LAB!! *****

## Lab 9 – Security Center

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

# ***** DO NOT END THE LAB!!  After completing Lab 9 use the drop-down window at the top to move to lab 10.  Do not end the lab!! *****<br>

## Lab 10: Azure Sentinel

Task 2: Configure Azure Sentinel to use the Azure Activity data connector<br>
Step 10:  Per the note it may take anywhere from 10-30 minutes before the connector shows Connected. Please wait for it to show Connected before proceeding.<br>

Task 4: Create a playbook<br>
Steps 1-3: Do these tasks in the VM, not your local OS.<br>

Task 5: Create a custom alert and configure a playbook as an automated response<br>
Step 10: Under Alert automation, select the drop-down and check the Select all box<br>

Task 6: Invoke an incident and review the associated actions<br>
For Steps 1-3, disable JIT VM access for myVM using the steps in Lab 14 Task 3<br>
Step 5: This can take several minutes to show up. Stretch & hydrate!<br>
