<h1>Implementing Auditing Policies in Windows</h1>

 ## [Video Demonstration (10:49)](https://drive.google.com/file/d/1rgUDLMHP2087eCGgObMZ72l-cCYP92A1/view?usp=sharing)

<h2>Description</h2>

This lab focuses on configuring and verifying auditing policies in Windows to enhance security monitoring and compliance. Key tasks include:<br/>

- Capturing running processes using `tasklist` for audit logging.
- Retrieving and analyzing file ACLs with `Get-Acl` to assess access permissions.
- Enabling **"Audit File System"** policy to log successful and failed file access attempts.
- Reviewing security logs in **Event Viewer** for unauthorized access detection.

This lab aligns with compliance standards like **ISO 27001 and PCI DSS** by implementing security auditing controls.


<h2>Lab walk-through:</h2>

<p align="left">The following command in Windows PowerShell lists all currently running processes and services on the system and saves the output to a file (C:\running_processes.txt) :<br/>

- Auditors can use this to verify that only authorized services are running.
- Can be compared against system policies to ensure compliance with security guidelines.
<br/>
<p align="center"><img src="https://i.imgur.com/yf19aHQ.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
<br/>
<img src="https://i.imgur.com/Y0VrFft.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center"><img src="https://i.imgur.com/YAof37E.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
<br/>
<img src="https://i.imgur.com/VRmk3yu.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center"><img src="https://i.imgur.com/Z0Ll50H.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
<br/>
<img src="https://i.imgur.com/0epTJem.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
