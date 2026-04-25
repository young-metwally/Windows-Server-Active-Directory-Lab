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

<img width="1023" height="772" alt="windows-server-2022-installation" src="https://github.com/user-attachments/assets/f4bee3aa-c1f2-4139-8d36-2f6b4b5721d1" />

---

### Configured Active Directory and DNS
The AD DS and DNS roles were installed and configured on the server. The `lab.local` domain was created and the domain controller `DC01` was confirmed running in both Active Directory Users and Computers and DNS Manager.

<img width="1015" height="766" alt="ad-and-dns-manager" src="https://github.com/user-attachments/assets/70bc6cca-7430-4df0-a119-681cc3f07fb6" />

---

### Verified Server Roles in Server Manager
The Server Manager dashboard was used to confirm that AD DS and DNS roles were installed and running without any issues.

<img width="1007" height="800" alt="server-manager-after-ad-ds-and-dns-setup" src="https://github.com/user-attachments/assets/235c72b7-992e-49a3-b5b3-f8ed04fb303c" />

---

### Logged In as Domain Administrator
After setup was complete, the domain controller was accessed using the `LAB\Administrator` account to begin configuring the environment.

<img width="1000" height="836" alt="login-screen-lab-administrator" src="https://github.com/user-attachments/assets/86c2442c-1591-4478-b7a2-06eeba1db922" />

---

### Created a HelpDesk Organizational Unit
A HelpDesk Organizational Unit was created inside Active Directory under the `lab.local` domain to organize users by department.

<img width="1020" height="712" alt="helpdesk-ou-created" src="https://github.com/user-attachments/assets/75f51950-a272-4cc0-985a-c2be10dc0e75" />

---

### Created a User Account
A `Test User` account was created inside the HelpDesk OU to simulate a real employee being onboarded into the system.

<img width="996" height="741" alt="user-created" src="https://github.com/user-attachments/assets/9559bf11-dc63-4955-aa2b-13971e2a0385" />

---

### Applied Password Policy
The user account was configured to require a password change at first login, simulating a standard onboarding security practice.

<img width="1013" height="746" alt="mustchangepass-testuser" src="https://github.com/user-attachments/assets/7bf52427-1ff1-4de1-a738-be8ddf0c8664" />

---

### Tested Password Policy on Login
The test user was logged into the domain and the password change prompt appeared as expected, confirming the policy was applied correctly.

<img width="1010" height="857" alt="asking-usertochangepass" src="https://github.com/user-attachments/assets/f3703885-0cfe-4ffc-ad32-b4f0ca36978a" />

---

### Password Successfully Changed
The test user completed the password change on first login, confirming the full policy flow worked end to end.

<img width="1006" height="752" alt="changepass" src="https://github.com/user-attachments/assets/1d9bf54e-6337-47c7-9975-14708bd135a7" />

---

## Skills Demonstrated

- Windows Server 2022 installation and configuration
- Active Directory setup and user management
- DNS configuration
- Group Policy creation and enforcement
- Network configuration with static IPs
- Domain joining and client-server connectivity
- Troubleshooting domain login issues
