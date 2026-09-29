<H1/> Active Directory Lab </H1>
This was a home lab that was done to demonstrate and replicate a small enterprise Windows environment using Active Directory Domain Services, Group Policy, Organizational Units, Security Groups, User Accounts, and a Windows 11 workstation that was joined to the domain.
<br/>

<H2/> Objective </H2>
I began this project to build and secure a functional Windows domain environment to develop practical experience with technologies encountered in enterprise IT and cybersecurity enviroments.
<br/>

<H2/> Skills Learned </H2>
-Active Directory Domain Services <br/>
-Windows Server Administration <br/>
-Organizational Units and Security Groups <br/>
-Group Policy <br/>
-Password and Account Lockout <br/>
-User and Computer Account Management <br/>
-Domain Authentication <br/>
-Security Validation <br/>
<br/>

<H2/> Tools Used </H2>
-Windows Server 2022 Core (DC) <br/>
-Windows 11 Pro (Client Computer) <br/>
-VirtualBox (Virtualization)
<br/>
<br/>

<H2/> The Project </H2>

<H3/> The Enviroment </H3>
DC01: Windows Server 2022 Core <br/>
-Active Directory <br/>
-DNS <br/>
-Group Policy <br/>
-IP:192.168.56.10 <br/>
-Subnet:255.255.255.0 <br/>
-DNS:192.168.56.10 <br/>
- <br/>
Internal Network <br/>
- <br/>
CLIENT01 <br/>
-Domain Joined <br/>
-RSAT Tools <br/>
-Domain: corp.local <br/>
-IP: 192.168.56.20 <br/>
-Subnet: 255.255.255.0 <br/>

<H3/> What I built </H3>
Active Directory <br/>
-Installed and Configured Active Directory Domain Services <br/>
-Created the domain (corp.local) <br/>
-Configured DNS <br/>
-Created Organizational Units <br/>
-Created Employee User Accounts <br/>
-Created Security Groups <br/>
-Assigned Users to Appropriate Groups <br/>
-Organized Workstation Accounts <br/>
<br/>
Windows Client <br/>
-Installed Windows 11 Pro <br/>
-Configured Networking and DNS <br/>
-Joined CLIENT01 to the Domain (corp.local) <br/>
-Installed and Configured RSAT Management Tools <br/>
-Verified Domain Authentication <br/>

<H3/>Security Configurations</H3>
Created and configured a workstation security baseline <br/>
-Established a hardened defensive starting point and minimizing exposure to baseline attack vectors. <br/>
Configured password requirements <br/>
-Mandates a minimum password length and complexity.<br/>
Configured password history <br/>
-Prevents users from using weak or compromised passwords when prompted for a password change. <br/>
Configured maximum password age <br/>
-Ensures passwords expire to limit password lifetime and promote constant password change. <br/>
Configured account lockout treshold <br/>
-Automatically locks an account after a specified number of failed attempts. <br/>
Configured account lockout duration <br/>
-Controls how long an account remains unusable after a lockout is triggered. <br/>
Configured auditing <br/>
-Enables detailed logging for system events. <br/>
Verified applied group policies <br/>
-Validates that security settings are successfully deployed through Group Policy Objects and are enforced on endpoints. <br/>

<H3/> Validation <H3/>
<H4/> 1.) Environment and Server Setup </H4>
Initial Deployment of the Windows Server VM in VirtualBox
<img width="1920" height="1080" alt="Running Window Server" src="https://github.com/user-attachments/assets/a5865d9c-4298-4d64-a79e-bba426f61051" />

Renaming Server to DC01 and System Info
<img width="1024" height="768" alt="Server-Rename-DC01" src="https://github.com/user-attachments/assets/ceff3fd9-5282-4777-9130-5168abc95f7b" />
<img width="1024" height="768" alt="Final-Sys-Info" src="https://github.com/user-attachments/assets/123f78df-36ca-4ced-afd6-68dc0fa2b219" />

Network Setup that Shows Static IP Addressing
<img width="1920" height="1080" alt="HO-Network-Config" src="https://github.com/user-attachments/assets/5d918cf4-2431-4599-a975-77744de1b3a3" />
<img width="1024" height="768" alt="Final-Network-Config" src="https://github.com/user-attachments/assets/ba33c76b-00fc-4698-8afa-6978250abdc5" /> 

<H4/> 2.) Active Directory Deployment and Verification </H4>
Successful Installation of Active Directory and Domain Services
<img width="1024" height="768" alt="Installed AD DS" src="https://github.com/user-attachments/assets/4b65435e-a3a2-4b09-b380-bae1c8c7b8ed" />
Domain Controller Promotion Confirmation
<img width="1024" height="768" alt="Verified DC" src="https://github.com/user-attachments/assets/ff5ae296-cf8d-4c5c-b35d-d41692467bd4" />
AD DS Service Operational Status
<img width="1024" height="768" alt="Verify AD Services" src="https://github.com/user-attachments/assets/6dd6e531-4b10-421b-a9f7-b8fbf0d98baf" />
DNS Zone and Record Creation for Domain Name Resolution
<img width="1024" height="768" alt="Test Connectivity" src="https://github.com/user-attachments/assets/128953c9-f2e2-47e5-b622-3fa56f43b2b1" />
<img width="1024" height="768" alt="Check DNS Records" src="https://github.com/user-attachments/assets/cb67a803-0048-4953-9f6a-4027c1e72b5e" />

<H4/> 3.) Client Workstation Provisioning </H4>
Deployment of the Windows Client Virtual Machine
<img width="1920" height="1080" alt="Creating CLIENT01" src="https://github.com/user-attachments/assets/ae1d41f2-047d-4bcb-a84a-a4636bb36a6b" />
<img width="1024" height="768" alt="Verifying CLIENT01" src="https://github.com/user-attachments/assets/17bc16ea-e664-405a-90e2-f53d833ae53d" />

<H4/> 4.) Active Directory Structure and User Administration </H4>
Organizational Unit Structure Representing the Enterprise Departments
<img width="1024" height="768" alt="OU Hierarchy" src="https://github.com/user-attachments/assets/4b7fac81-98ea-41bb-baea-efd687229bc9" />
Populating the Department Security Groups with Domain Accounts
<img width="1024" height="768" alt="Add Employees to Groups" src="https://github.com/user-attachments/assets/27f3547a-d06a-4b19-be7f-1c37f42eae46" />
Final Layout for the Organization
<img width="1024" height="768" alt="Complete Account Organization" src="https://github.com/user-attachments/assets/2256e789-694b-44bc-93b0-a171c2a1a7b0" />

<H4/> 5.) Group Policy Hardening and Enforcement </H4>
Creating Security GPO
<img width="1024" height="768" alt="Creating Security GPO" src="https://github.com/user-attachments/assets/bbb756bc-80a9-428f-be02-457233f45489" />
Account Lockout Policy
<img width="1024" height="768" alt="Account Lockout Policy" src="https://github.com/user-attachments/assets/4f7101a5-a698-4908-8bba-45f95f250810" />
Audit Policy
<img width="1024" height="768" alt="Audit Policy" src="https://github.com/user-attachments/assets/93609119-c93d-4df6-98ba-1c93bc1bb3ae" />
Password Policy
<img width="1024" height="768" alt="Password Policy" src="https://github.com/user-attachments/assets/760ebcb8-8605-47c4-92f7-00f3d0dd1359" />
User Rights Policy
<img width="1024" height="768" alt="User Rights Policy" src="https://github.com/user-attachments/assets/ed17d5f3-0858-4231-b254-de77cdcff246" />
Automatic Updates
<img width="1024" height="768" alt="Automatic Updates" src="https://github.com/user-attachments/assets/7d482e0f-88f6-4fad-91e3-df98eb9db290" />
Logging Settings
<img width="1024" height="768" alt="Logging Settings" src="https://github.com/user-attachments/assets/b29ddb8b-9938-4c0b-a088-e559c2f279e4" />
Windows Firewall Defender
<img width="1024" height="768" alt="Windows Firewall Defender" src="https://github.com/user-attachments/assets/7c54076e-bd58-4374-9a5f-06fc9b09565f" />
Group Policy Verified
<img width="1024" height="768" alt="Group Policy Verified" src="https://github.com/user-attachments/assets/613bfec6-c192-47ab-881b-6907b9cb05b5" />
Applied GPO
<img width="1024" height="768" alt="Applied GPO" src="https://github.com/user-attachments/assets/c44f1a82-3998-4515-9320-a07b11101004" />

<H4/> 6.) Event Logging and Security Auditing </H4>
Account Creation Event
<img width="1024" height="768" alt="Account Creation Event" src="https://github.com/user-attachments/assets/51eb73ac-36b4-4986-acb8-9fc46bfa3b34" />
Successful Logon Event
<img width="1024" height="768" alt="Successful Logon Event" src="https://github.com/user-attachments/assets/3d1ac819-2c08-4418-a242-a33ce44ebd51" />
Failed Logon Event
<img width="1024" height="768" alt="Failed Logon Event" src="https://github.com/user-attachments/assets/b4596653-bda6-43b1-b078-ed49f50bc505" />
Security Group Change Event
<img width="1024" height="768" alt="Security Group Change Event" src="https://github.com/user-attachments/assets/20f92946-80b5-43e5-b26a-e430fcde541a" />

<H4/> 7.) Final Verification </H4>
Firewall Verification
<img width="1024" height="768" alt="Firewall Verification" src="https://github.com/user-attachments/assets/c47b2691-a518-4dc1-a0b4-0cf66122080f" />
System Audit Policy
<img width="1024" height="768" alt="System Audit Policy" src="https://github.com/user-attachments/assets/3e54f4d9-9697-4927-b605-366524599889" />
Antivirus and Antispyware
<img width="1024" height="768" alt="Verify Antivirus and Antispyware" src="https://github.com/user-attachments/assets/d64544f6-f7e8-4de5-b554-8d97ce0d2db5" />
Audit Policy
<img width="1024" height="768" alt="Verify Audit Policy" src="https://github.com/user-attachments/assets/8622a0bd-4812-4ad6-a0de-0cc3f9193576" />
Password Changes
<img width="1024" height="768" alt="Verify Password Changes" src="https://github.com/user-attachments/assets/479ed018-e60f-4431-8589-e862b8b3ce67" />
Active Directory and Domain Connectivity
<img width="1024" height="768" alt="Final Validation (AD and Domain Connectivity)" src="https://github.com/user-attachments/assets/93abf9b7-7f91-45ce-828e-de837775869f" />
Domain Trust
<img width="1024" height="768" alt="Final Validation (Domain Trust)" src="https://github.com/user-attachments/assets/128b67a7-8f54-4cab-880b-3f58e705c57f" />

<br/>
<H2> Troubleshooting/Issues </H2>
Not sufficient RAM to support the Windows Pro 11 client <br/>
- <br/>
DNS configuration initially pointed to the wrong DNS server <br/>
- <br/>
Group Policy initially appeared not to apply <br/>
- <br/>
%userdomain% was not returning the expected domain <br/>
- <br/>
Issues relating to existing users and organizational units <br/>
- <br/>
Troubleshooting domain authentication and policy application <br/>
- <br/>
Verifying the domain relationship between CLIENT01 and DC01 <br/>
- <br/>

<br/>
<H2> Lessons Learned </H2>









