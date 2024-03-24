# AZ-500T00 Learning Path 1 Labs Errata   
 
Updated January 2022, November and September 2021 - Labs are the same as July 2020 revision <br> 

When starting each lab choose Yes when prompted to be visible in networks<br> 

# Remember anywhere the term Azure Active Directory (AAD) select Microsoft Entra ID  (Name change)

## Lab 1 – Role-Based Access Control ~30 Minutes (90 Min)

### Exercise 2 – Create a Junior Admins group containing the user account Isabel Garcia as its member

Task 1: <br>
Step 1:  PowerShell is now called Windows Terminal (Admin) when right clicking on the start menu.<br>
Step 2:  When copying and pasting command it sometimes pastes wrong, Ensure the command is Install-Module <br>
Add the following command before befroe step 7 <br>
$domainname = "M365x60893010.mail.onmicrosoft.com" <br>
Note - copy the UPN from the the Joseph user you created in Exercise 1 - just the UPN not the entire it should look something like this M365x60893010.mail.onmicrosoft.comname <br>

### Exercise 3 – Creating a Service Desk Group; containing the user account Dylan Williams as its member

Task 1: Use Azure CLI to create a user account Dylan Williams<br> 
If you encounter an error during this lab that indicates the clock is out of sync or the current time is in error, use the Settings app in the VM to synchronize the computer’s clock and then retry the step<br>
Wait for step 1 to complete before moving on to step 2 <br>
After running step 3 choose Edge Browser and enter your Azure tenant admin account and password <br>

## Labs 2 and 3: MFA, Conditional Access and AAD Identity Protection & Privileged Identity Management (PIM) ~60 minutes (6 Hours) 

Before completing this lab create an outlook.com account for use in this lab.  Refer to the create an outlook.com account document in the file share.<br>

