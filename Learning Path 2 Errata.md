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

# Learning Path 2 Additional Labs ~240 Minutes (360 Min)

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
Step 2:  If you get an error the Subnet Address Range cannot be blank.  Populate it with the IP Adress from Task 3 > Step 2 > Public IP Addresss range provided in the box <br>

Task 6:  Create an NVA <br>
Step 8:  Select - “Enable with custom storage Account” <br>
Use the name that auto populates <br>

Task 7: Turn on IP forwarding <br>
Step 4:  Select Apply <br>

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


