<h2>Program walk-through:</h2>

Download Nessus: <br/>
<img src="https://i.imgur.com/4aS7VfQ.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
    
Configure and Install Nessus:  <br/>
<img src="https://i.imgur.com/hf3Ynbw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Start Nessus: <br/>
<img src="https://i.imgur.com/wiytxVs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to the Nessus web interface and select continue: <br/>
<img src="https://i.imgur.com/HXz5oI1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Register for Activation Code: <br/>
<img src="https://i.imgur.com/5kmr6Eg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/RZV79af.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create User: <br/>
<img src="https://i.imgur.com/sbsaW1u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for the plugins to finish downloading: <br/>
<img src="https://i.imgur.com/2Gy2YNp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/1IowZTt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />



<h2>Credentials Scan Configuration</h2>
The company’s security policies require Linux systems to be regularly audited for vulnerabilities.

Select Credential Patch Audit to perform the scan: <br/>
<img src="https://i.imgur.com/GoavWFi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
1. In the Credentials tab, select SSH

2. Set the Username to root.

3. In the Password field, enter kali (for Kali Linux users) or the password for the
root account (for Ubuntu users if applicable).

4. For Elevate Privileges, choose "su".
Set Custom Password Prompt to password.

5. Use the command ssh -V to check for the version of OpenSSH running on the
system and input that into the scan configuration: <br>
<img src="https://i.imgur.com/YG5Uryi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/xi0QpKn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<h2>Web Application Vulnerabilty  Scan:</h2>
The IT team wants to assess the security of a web application running on the Linux server. Your
objective is to perform a web application scan using Nessus.

In Nessus, create a Web Application Test scan.
<img src="https://i.imgur.com/qdgaNRm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Use the default scan settings without configuring authentication
<img src="https://i.imgur.com/JooSLpK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<h2>Email Configuration for Automated Reporting:</h2>
The IT team requires that Nessus send automated email reports after each scan. You are
tasked with configuring Nessus to send these reports using Gmail’s SMTP server.
<img src="https://i.imgur.com/dHNKnfp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
In the Nessus Settings tab, select SMTP.
<img src="https://i.imgur.com/h1XGfZj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Launch the scan
<img src="https://i.imgur.com/aMc8Hku.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<h2>CVE Research and Analysis:</h2>
Upon completing the scans, Nessus will detect certain Common Vulnerabilities and Exposures
(CVEs) in the Linux system and web application. Conduct research on the CVEs identified in the
scan results to understand the risks they present, possible exploitation methods and their
potential impact.
<img src="https://i.imgur.com/xQIUsry.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/eUL7Ipd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src=https://i.imgur.com/D97eAe5.pngg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/biuaZT5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/MclRM1L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/VrnKhTA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/uYJS5A3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/bT4CbYz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
