<h1>Extracting and Exploring IoT Firmware</h1>
<h2>*FOR EDUCATIONAL PURPOSES ONLY*</h2>



<h2>Description</h2>
In this project I used Binwalk, a firmware reverse engineering tool, on a VM running AttifyOS, an IoT offensive security OS, to extract and explore publicly available firmware. The purpose of this project is to identify and assess potential vulnerabilities in the firmware of an embedded device for eventual management and mitigation of determined risk.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Binwalk</b> 

<h2>Environments Used </h2>

- <b>AttifyOS</b>
- <b>Oracle VirtualBox</b>

<h2>Learning Outcomes</h2>

- <b>Use of OSINT for security research</b>
- <b>Assessment of potential vulnerabilities in embedded device</b>
- <b>Binwalk utility syntax and features</b>
- <b>Firmware filesystem enumeration</b>
- <b>Exposure to AttifyOS, an open source IoT Offensive Security OS</b>
  
<h2>Project walk-through:</h2>

<p align="center">
Download publicly available IoT firmware: <br/>
<img src="https://i.imgur.com/cbeIvHz.png" height="80%" width="80%" alt="IoT Firmware Download"/>
<br />
<br />
Initial Binwalk Analysis: *note enumeration of squashfs filesystem*  <br/>
<img src="https://i.imgur.com/Opwk0WO.png" height="80%" width="80%" alt="Binwalk Initial Analysis"/>
<br />
<br />
Encryption Check: *indicates no encryption* <br/>
<img src="https://i.imgur.com/9at2FbE.png" height="80%" width="80%" alt="Encryption Check"/>
<br />
<br />
Firmware Extraction: *note 'extracted' binary*  <br/>
<img src="https://i.imgur.com/E29hoBa.png" height="80%" width="80%" alt="Firmware Binary Extraction"/>
<br />
<br />
Firmware Filesystem Enumeration: *note default credentials*  <br/>
<img src="https://i.imgur.com/NFd9ExP.png" height="80%" width="80%" alt="Filesystem Enumeration"/>
<br />
<br />
Initialization Script: *potential attack surface*  <br/>
<img src="https://i.imgur.com/jQUHa8f.png" height="80%" width="80%" alt="Initialization Script"/>
<br />
<br />
Root Enumeration:  <br/>
<img src="https://i.imgur.com/sZ4Q0TX.png" height="80%" width="80%" alt="Root Enumeration"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
