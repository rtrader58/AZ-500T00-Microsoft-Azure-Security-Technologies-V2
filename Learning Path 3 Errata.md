# AZ-500T00 Learning Path 3 Errata (2020 revision) 

Updated November and September 2021 - Labs are the same as July 2020 revision <br>
When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

# Learning Path 3 - Secure Data and Applications ~150 Minutes (180 Min)

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

## Lab 6 – Service Endpoints and Securing Storage ~55 Minutes (60 Min)

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
