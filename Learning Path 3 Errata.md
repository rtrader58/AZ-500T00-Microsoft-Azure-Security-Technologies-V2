# AZ-500T00 Learning Path 3 Errata (2024 revision) 

When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

# Learning Path 3 - Secure Data and Applications - Total lab time ~180 Minutes (270 Min)

## Lab 4 – Configuring and Securing ACR and AKS ~60 Minutes (90 Min)

### Exercise 1:  Configuring and Securing ACR and AKS

Task 1:  Create an Azure Container Registry <br>
Step 2:  Open the Cloud Shell by clicking the first icon in the top right of the search area in the Azure portal > Select Bash > click Mount Storage Account > in the drop down choose your subscription > click Apply > select We will create a storage account for you > click next <br>
Once the CloudShell opens click on Setting and select Go to classic version <br>

Task 3: Create an Azure Kubernetes Service cluster<br>
Step 6:  Do not continue until the cluster is complete<br>
Step 10:  The Azure Kubernetes Service Cluster is inside the AZ500Lab09 Resource Group <br>
After step 10 - Create the required Vnet using the following steps <br>
Search for Virtual network <br>
Click Create <br>
Use the provided Resource Group <br>
Nme the Vnet:  AZ500LAB09-vnet <br>
Select Review+Create, then Create <br>

Task 4:  Give AKS permissions to access the ACR <br>
Step 2:   Look in your resources group to see the name of the container registry, replace <ACRuniquename> with the container name <br>

Task 5: Deploy an external service to AKS<br>
Step 1:  Click on Manage files > Upload > the allfils folder is on the desktop <br>
Step 3:  If prompted to return to previous Cloud shell click Confirm > repaste Step 3 <br>
Step 5: There no ellipses. Move your cursor to the upper right hand corner of the editor and left click you will see the option to save and also option to close.<br>
Skip Step 7 <br>

Task 7: Deploy an internal service to AKS <br>
Skip step 5 <br>

## Lab 5 – Securing Azure SQL Database ~45 Minutes (90 Min)

Task 1: Deploy an Azure SQL Database <br>
Step 4:  Allfiles is located on the Desktop <br>

## Lab 6 – Service Endpoints and Securing Storage ~75 Minutes (90 Min)

### Exercise 1: Service endpoints and security storage

Task 3: Configure a network security group to restrict access to the subnet <br>
step 10:  Search for Network Security Group > Click on MyNsgPrivate > Settings 

Task 5: Create a storage account with a file share <br>
Step 3:  Use the existing Resource Group <br>
Steps 9 and 10 are reversed <br>
Step 18 Click Enable, then click Add

Task 6: Deploy virtual machines into the designated subnets
Step 3:  Use the existing Resource Group <br>
Step 3:  For the password I used the Azure Admin passowrd in the resources tab.  I had to add 123 at the end to get 12 characters <br>
Step 9:  Use the existing Resource Group <br>
Step 9:  For the password I used the Azure Admin passowrd in the resources tab.  I had to add 123 at the end to get 12 characters <br>

Clean up resources <br>
Delete the AZ500LAB12 Resource Group <br>

