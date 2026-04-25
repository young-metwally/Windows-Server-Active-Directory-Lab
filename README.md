# IT Help Desk Lab

A hands-on home lab built using VirtualBox to simulate a real IT environment. This project covers setting up a Windows Server 2022 domain controller, configuring Active Directory, managing users and group policies, and connecting a Windows 10 Pro client to the domain.

---

## Tools & Technologies

- Oracle VirtualBox
- Windows Server 2022
- Windows 10 Pro
- Active Directory Domain Services (AD DS)
- DNS Manager
- Group Policy Management

---

## What I Did

### Installed Windows Server 2022
Windows Server 2022 was installed as a virtual machine inside VirtualBox to serve as the domain controller for the lab environment.

<img width="600" alt="windows-server-2022-installation" src="https://github.com/user-attachments/assets/493ecfc0-3418-4b0f-8cce-b50748cde611" />

---

### Configured Active Directory and DNS
The AD DS and DNS roles were installed and configured on the server. The `lab.local` domain was created and the domain controller `DC01` was confirmed running in both Active Directory Users and Computers and DNS Manager.

<img width="600" alt="ad-and-dns-manager" src="https://github.com/user-attachments/assets/83488e5b-b756-4985-bd63-cff399a56f1f" />

---

### Verified Server Roles in Server Manager
The Server Manager dashboard was used to confirm that AD DS and DNS roles were installed and running without any issues.

<img width="600" alt="server-manager-after-ad-ds-and-dns-setup" src="https://github.com/user-attachments/assets/a1cb97a6-1f55-4654-bab8-84e3536c18f9" />

---

### Logged In as Domain Administrator
After setup was complete, the domain controller was accessed using the `LAB\Administrator` account to begin configuring the environment.

<img width="600" alt="login-screen-lab-administrator" src="https://github.com/user-attachments/assets/b7063849-81ed-4c89-ae0c-e9b7b8d329e7" />

---

### Created a HelpDesk Organizational Unit
A HelpDesk Organizational Unit was created inside Active Directory under the `lab.local` domain to organize users by department.

<img width="600" alt="helpdesk-ou-created" src="https://github.com/user-attachments/assets/59c0db5c-53ba-4de8-be41-282a3afe53da" />

---

### Created a User Account
A `Test User` account was created inside the HelpDesk OU to simulate a real employee being onboarded into the system.

<img width="600" alt="user-created" src="https://github.com/user-attachments/assets/178a5610-c7b6-43a2-bd9c-e2ea9f048eb5" />

---

### Applied Password Policy
The user account was configured to require a password change at first login, simulating a standard onboarding security practice.

<img width="600" alt="mustchangepass-testuser" src="https://github.com/user-attachments/assets/0ea27f58-4b71-456a-9bde-f12b0fd45b49" />

---

### Tested Password Policy on Login
The test user was logged into the domain and the password change prompt appeared as expected, confirming the policy was applied correctly.

<img width="600" alt="asking-usertochangepass" src="https://github.com/user-attachments/assets/a867696c-ed85-400f-a774-1316f638de72" />

---

### Password Successfully Changed
The test user completed the password change on first login, confirming the full policy flow worked end to end.

<img width="600" alt="changepass" src="https://github.com/user-attachments/assets/0c15fed3-09f5-4eaa-bda7-9af82de395ee" />

---

## Skills Demonstrated

- Windows Server 2022 installation and configuration
- Active Directory setup and user management
- DNS configuration
- Group Policy creation and enforcement
- Network configuration with static IPs
- Domain joining and client-server connectivity
- Troubleshooting domain login issues
