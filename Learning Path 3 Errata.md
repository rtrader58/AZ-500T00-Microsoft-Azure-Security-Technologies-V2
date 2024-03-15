# AZ-500T00 Learning Path 3 Errata (2020 revision) 

Updated November and September 2021 - Labs are the same as July 2020 revision <br>
When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

# Learning Path 3 - Secure Data and Applications ~150 Minutes (180 Min)

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

## Lab 10 – Key Vault ~75 Minutes (60 Min)

## Exercise 2: Configure the Key Vault resource with a key and a secret

Task 1: Create and configure a Key Vault
Step 11:  in the resources pane of the resource group, select the keyvault you just created 

## Exercise 3: Configure an Azure SQL database and a data-driven application

Task 2: Create a policy allowing the application access to the Key Vault<br>
Step 3:  Replace  ‘<Azure_AD_Application_Id>’ with your AP ID recorded in earlier step.  Make sure to include the ‘ at the beginning and end<br>

Task 5: Create a table in the SQL Database and select data columns for encryption
Step 10:  If you get an error when connecting, manually type in your password

Step 14:  If the paste does not paste correctly, open notepad on the Lab VM not the RDP session and paste the query into notepad.  Copy and paste from notepad into the the RDP session
