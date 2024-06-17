# AZ-500T00 Learning Path 2 Labs Errata

When starting each lab choose Yes when prompted to be visible in networks<br>

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 2 – Network Security Groups and Application Security Groups ~45 Minutes (60 Min) 

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
