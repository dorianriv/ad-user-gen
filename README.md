<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Project Logo"/>
</p>

<h1>Active Directory: User and Group Management – Phase 3</h1>

<p>
In this phase of the Active Directory lab series, we’ll use PowerShell to bulk-create users in our domain. This allows us to populate our environment efficiently and prepare for group management and access control testing in the next phase.
</p>

<h2>Overview</h2>

<p>
Building on our existing AD setup, this phase focuses on:

- Creating multiple user accounts using a PowerShell script
- Verifying user creation in Active Directory
- Logging in as one of the generated users to confirm success

By the end of this phase, we’ll have a working pool of domain users for future simulations.
</p>

<h2>Key Objectives</h2>

<h3>User Generation</h3>
- Use a PowerShell script to create multiple domain users

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)  
- Active Directory Domain Services  
- PowerShell  
- Remote Desktop

<h2>Operating Systems Used</h2>

- Windows Server 2022  
- Windows 10 (21H2)

<h2>Configuration Steps</h2>

<h3>&#9312; Run the PowerShell Script</h3>

- Log in to DC-1 as jane_admin
- Open PowerSell ISE as an administrator and paste the contents of the <a href="https://github.com/joshmadakor1/AD_PS/blob/master/Generate-Names-Create-Users.ps1"> script </a> and run it

![screenshot 1](https://github.com/user-attachments/assets/26a33215-e783-49cb-92bc-89e4b433c1c9)

- The script will generate several users with a combination of consonants and vowels, so the names might be unusual

- Once the script is done running, you can verify in Active Directory that the users have been created

![screenshot 2](https://github.com/user-attachments/assets/ed48499a-0051-4207-be8b-fdb4ac7fdaef)

<h3>&#9313; Login as a user</h3>

- Now you can try logging in as one of the users to further verify that the script has worked
- Take note of the default password in the script (Password1)

![screenshot 3](https://github.com/user-attachments/assets/67704ee6-b881-4f56-ba2f-371a3aedbb8e)

<h2>Final Thoughts</h2>

<p>
Using an automated PowerShell script, we’ve successfully added multiple users to our domain. This will make testing access control and simulating group-based permissions easier in the next and final phase: Simulating Real-World Active Directory Scenarios.
</p>
