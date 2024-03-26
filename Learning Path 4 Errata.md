# AZ-500T00 Learning Path 4 Labs Errata  – Total time ~210 hours 

When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 7 – Key Vault ~75 Minutes (60 Min)

## Exercise 2: Configure the Key Vault resource with a key and a secret

Task 1: Create and configure a Key Vault
Step 11:  in the resources pane of the resource group, select the keyvault you just created 

## Exercise 3: Configure an Azure SQL database and a data-driven application

Task 2: Create a policy allowing the application access to the Key Vault<br>
Step 3:  Replace  ‘<Azure_AD_Application_Id>’ with your AP ID recorded in earlier step.  Make sure to include the ‘ at the beginning and end<br>

Task 5: Create a table in the SQL Database and select data columns for encryption
Step 10:  If you get an error when connecting, manually type in your password

Step 14:  If the paste does not paste correctly, open notepad on the Lab VM not the RDP session and paste the query into notepad.  Copy and paste from notepad into the the RDP session

# NOTE - Lab 8, 9 and 10 launch in a single lab environment - Do Note End between labs

## Lab 8 – Azure Monitor ~30 Minutes

Task 3: Enable the Log Analytics virtual machine extension <br>
Step 1: Before beginning this task, ensure that the Log Analytics Workspace deployment has completed successfully, it should take 1-2 minutes<br>
Step 2 – if the VM is not listed, wait a few minutes and then refresh the view. It can take up to 15 minutes for the VM to appear in the list. Also, verify that the VM you created in Task 1 is Running.<br>
Step 4 - 5: It can take a few minutes to connect.  (On 11/5/2021 this took 2.5 minutes) This is a great time to stretch & hydrate!<br>

Task 5: View and query collected data<br>
Step 3: Close the video in the details section of this page, and ignore the instruction to click “get started”<br>
Step 4: Navigate to the Virtual Machines queries in the All Queries column or use Search<br>
Step 5: It doesn’t matter which queries you run, this task is to show you VM log data being gathered. Note that some queries will have no results as not enough data has been gathered yet.<br>

# ***** DO NOT END THE LAB!!  After completing Lab 11 use the drop down window at the top to move to lab 12  DO NOT END THE LAB!! *****

## Lab 9 – Security Center ~60 Minutes

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

# ***** DO NOT END THE LAB!!  After completing Lab 12 use the drop-down window at the top to move to lab 13.  Do not end the lab!! *****<br>

## Lab 10: Azure Sentinel ~45 Minutes

Task 2: Configure Azure Sentinel to use the Azure Activity data connector<br>
Step 10:  Per the note it may take anywhere from 10-30 minutes before the connector shows Connected. Please wait for it to show Connected before proceeding.<br>

Task 4: Create a playbook<br>
Steps 1-3: Do these tasks in the VM, not your local OS.<br>

Task 5: Create a custom alert and configure a playbook as an automated response<br>
Step 10: Under Alert automation, select the drop-down and check the Select all box<br>

Task 6: Invoke an incident and review the associated actions<br>
For Steps 1-3, disable JIT VM access for myVM using the steps in Lab 14 Task 3<br>
Step 5: This can take several minutes to show up. Stretch & hydrate!<br>
