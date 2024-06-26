# AZ-500T00 Learning Path 4 Labs Errata  – Total time ~210 hours 

When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 7 – Key Vault (Implementing Secure Data by setting up Always Encrypted) ~75 Minutes (90)

### Exercise 1: Deploy the base infrastructure from an ARM template

Task 1: Deploy an Azure VM and an Azure SQL database <br>
Step 4:  Allfiles is located on the Desktop <br>

## Exercise 2: Configure the Key Vault resource with a key and a secret

Task 1: Create and configure a Key Vault <br>
Replace steps 1 - 4 with the following steps. (Key vault has to be created manually) <br>
Search for Key Vaults, select Key Vaults for the list <br>
Clcik + Create <br>
Select the pre-created Resource Group <br>
Name the Key Vault - az500kv-yourinitials <br>
Click Next <br>
Under Permission model select the radial button next to Vault access policy <br>
Under Access policies ensure your user account is checked <br>
Click Review and create > Create <br>

Step 9:  After selecting the 15 Certificate permissions > Clcik next > on the Principal tab search for your account (paste user account into search from the Lab Resources tab

## Exercise 3: Configure an Azure SQL database and a data-driven application

Task 2: Create a policy allowing the application access to the Key Vault<br>
Step 3:  Replace  ‘<Azure_AD_Application_Id>’ with your AP ID recorded in earlier step.  Make sure to include the ‘ at the beginning and end<br>

Task 5: Create a table in the SQL Database and select data columns for encryption <br>
Step 6:  The link will open in your local browser > copy the link and paste into the Edge browser in the lab (installation took ~10 minutes) <br>
Step 10:  If you get an error when connecting, manually type in your password <br>

Step 16:  You may have to sign into Azure to see your key vault.  Click sign into Azure <br>

# NOTE - Labs 8, 9 and 10 launch in a single lab environment - Do Note End between labs ~180 Minutes (320)
### Keep an eye on the lab timer.  You will need to extend the lab at least once to complete 

## Lab 8 – Azure Monitor

### Exercise 1: Deploy an Azure virtual machine

Task 1: Deploy an Azure virtual machine
Step 6:  If you get an error the NRP service is not register.  Rerun the command <br>

# ***** DO NOT END THE LAB!!  After completing Lab 8 use the drop down window at the top to move to lab 9  DO NOT END THE LAB!! *****

## Lab 9 – Security Center

Task 1: Configure Security Center <br>
Step 1: You’re already logged in, you can skip this step<br>
Step 4: You may need to refresh the screen to see Install Agents

If JIT does not appear as an option within 30 minutes, move on to Lab 15.<br> It is not necessary to complete the JIT VM Access task to complete the labs.<br>

# ***** DO NOT END THE LAB!!  After completing Lab 9 use the drop-down window at the top to move to lab 10.  Do not end the lab!! *****<br>

## Lab 10: Azure Sentinel

Task 2: Configure Azure Sentinel to use the Azure Activity data connector<br>
Step 10:  Per the note it may take anywhere from 10-30 minutes before the connector shows Connected. Please wait for it to show Connected before proceeding.<br>

Task 3: Create a rule that uses the Azure Activity data connector <br>
Step 3:  You will need to split off the instructions and go full screen to see the scroll bar <br>

Task 4: Create a playbook<br>
Steps 1-3: Do these tasks in the VM, not your local OS.<br>

Task 5: Create a custom alert and configure a playbook as an automated response<br>
Step 10: Under Alert automation, select the drop-down and check the Select all box<br>

Task 6: Invoke an incident and review the associated actions<br>
Step 5: This can take several minutes to show up. Stretch & hydrate!<br>
