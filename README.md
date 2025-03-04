<h1>Implementing Auditing Policies</h1>

 ## [Video Demonstration (10:49)](https://drive.google.com/file/d/1rgUDLMHP2087eCGgObMZ72l-cCYP92A1/view?usp=sharing)

<h2>Description</h2>

This lab focuses on configuring auditing policies to enhance security monitoring and compliance. Key tasks include:<br/>

- Capturing running processes using `tasklist` for audit logging.
- Retrieving and analyzing file ACLs with `Get-Acl` to assess access permissions.
- Enabling **"Audit File System"** policy to log successful and failed file access attempts.

This lab aligns with compliance standards like **ISO 27001 and PCI DSS** by implementing security auditing controls.


<h2>Lab walk-through:</h2>

<p align="left">The command below lists all currently running processes and services on the system and saves the output to a file (C:\running_processes.txt) :<br/>

- Auditors can use this to verify that only authorized services are running.
- Can be compared against system policies to ensure compliance with security guidelines.
<br/>
<p align="center"><img src="https://i.imgur.com/yf19aHQ.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p align="center"><img src="https://i.imgur.com/FN6uQf3.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
<p align="left">The command below retrieves the Access Control List (ACL) permissions for the file Info_Sec.txt located in C:\ConfidentialData and saves it to C:\Info_SecPermissions.txt .
<br/>
<p align="center"><img src="https://i.imgur.com/Ind1G1s.png" height="70%" width="100%" alt="Disk Sanitization Steps"/>
<br/>
<p align="left">By opening the file we can observe  :<br/>

- Admin_Support has ReadAndExecute, meaning they can view but not modify the file.
- Administrators and SYSTEM have FullControl, which is normal.

<br/>
<p align="center"><img src="https://i.imgur.com/TzPKxoa.png" height="70%" width="100%" alt="Disk Sanitization Steps"/>

<p align="center">Next I will configure an audit policy in GPO (Group Policy Object).
<br/>
<p align="center"><img src="https://i.imgur.com/v1V8Lhi.png" height="70%" width="100%" alt="Disk Sanitization Steps"/>
<br/>
<p align="center">Enabling "Audit File System" policy to log successful and failed file access attempts.
<br/>
<p align="center"><img src="https://i.imgur.com/xZpMXeM.png" height="70%" width="100%" alt="Disk Sanitization Steps"/>
<br/>
<p align="center">Applying the policies:
<br/>
<p align="center"><img src="https://i.imgur.com/in6iWTK.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
 
