# NetworkWalks-B084D-week3-Crack-The-Password

| **Pentester Name / (Cybersecurity Professional)** | Elijah Cauyan |
| --- | --- |
| **Batch** | B084-Networkwalks |
| **Date** | November 17, 2026 |
| **Modules Completed** | W3-PM1 / W3-P2M |
| **Target** | Locked PDF files |
| **Permission secured from client?** | Yes |
<br> 

<div align="center">

**LIABILITY DISCLAIMER**

</div>

During this report, I have performed brute-force attack activities on locked files, for which I was given authorization to break into. All the steps and procedures shown in the report are al purely for educational purposes and must not be used to harm others or break the law. The instructors, authors, and Networkwalks are not responsible for what you do with this knowledge, and any action you take is your own responsibility; misuse of knowledge can lead to criminal charges, penalties, and a permanent record.
<br> 
<br> 

<div align="center">
  
**INTRODUCTION**

</div>

In this report, I will showcase how I completed the tasks that I was given for my third-week internship at Networkwalks, which are WK3-PM1 and WK3-PM2, which focus on password cracking, also known as brute-force attacks.

Additionally, this report will cover how to install and use different brute-force attack tools such as locked PDF hash converter, John the Ripper, johnny, and Networkwalks tools. This set of tools is used to brute-force multiple locked PDFs, which I was given authorization to break into.
<br> 
<br> 

<div align="center">
  
**TOOLS USED**

</div>

| **Tool** | **Purpose** |
| --- | --- |
| Kali Linux OS | Operating System used for brute-force attack tools and activities. |
| Linux Terminal | Provides Linux command-line functionality. |
| John the Ripper | Identifies and tests password hashes to assess password strength |
| Johnny GUI | Provides a graphical interface for John the Ripper. |
| Online hashing tool (https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php) | Extracts password hashes from PDF files. |
| Networkwalks Hash Calculator | Networkwalks’ tool that calculates the hash digest of the files. |
| Networkwalks Password Cracker | Networkwalks’ tool that cracks the file's password based on the hash inputed |

<br> 
<div align="center">


**Method 1: Using John the Ripper**

</div>

1. Downloaded and installed Johnny (the GUI front-end for John the Ripper).
2. Took a password-protected PDF file and generated its hash using a PDF-to-hash tool.
3. Copied the generated hash and saved it in a Notepad file.
4. Opened the command line/terminal and ran John the Ripper against the saved hash file.
5. John the Ripper processed the hash and recovered the original password of the file.
   
**Screenshots**

<img width="1487" height="812" alt="Screenshot 2026-11-19 145812" src="https://github.com/user-attachments/assets/874266b5-e284-433f-b2c3-950461af8a6b" />
<img width="1320" height="572" alt="Screenshot 2026-11-19 150112" src="https://github.com/user-attachments/assets/6f406bdf-ccb7-4344-b15e-747515945710" />
<img width="1362" height="686" alt="Screenshot 2026-11-19 150233" src="https://github.com/user-attachments/assets/7a00b618-3000-4781-90a2-e867e2fe4259" />
<img width="795" height="976" alt="Screenshot 2026-11-19 150251" src="https://github.com/user-attachments/assets/3acf0060-31df-40af-8557-fd67ddacd2fd" />

<br> 
<div align="center">


**Method 2: Using Network Walks Tools**

</div>

1. Uploaded the same file to the Network Walks online hash calculator to generate its hash value.
2. Copied the generated hash value.
3. Pasted the hash into the Network Walks online password cracker tool.
4. Ran a dictionary attack using the tool, which matched the hash against a wordlist.
5. The tool returned the original password of the file.

**Screenshots**

</div>

<img width="1125" height="722" alt="Screenshot 2026-11-19 191317" src="https://github.com/user-attachments/assets/69dcbdf8-b11b-4680-b530-c1ee3aa8981a" />
<img width="1488" height="951" alt="Screenshot 2026-11-19 191544" src="https://github.com/user-attachments/assets/68bf1983-1b46-43ce-90bb-34f2129c7f5c" />
<img width="750" height="977" alt="Screenshot 2026-11-19 191623" src="https://github.com/user-attachments/assets/4a2b3662-226e-4730-a291-e07b79b47525" />

<br> 
<div align="center">


**Comparison of the Two Methods**

</div>

| Aspect | John the Ripper (Local) | Network Walks (Online) |
|---|---|---|
| Setup | Requires installing Johnny/John the Ripper | No installation, browser-based |
| Processing | Done locally on the machine | Done on the tool's server |
| Attack type used | Command-line based cracking | Dictionary attack |
| Privacy | Hash stays on local machine | Hash is uploaded to a third-party site |

<br>
<div align="center">


**Reference Links**

</div>

-John The Ripper
 -Johnny CLI : *https://www.openwall.com/john/*
 -Johnny GUI: *https://openwall.info/wiki/john/johnny*
- Network Walks tool links used:
  - Hash calculator: *https://networkwalks.com/hash-calculator/*
  - Password cracker (dictionary attack): *https://networkwalks.com/password-cracker.com/*

<br>
<div align="center">


**Learnings**

</div>

1. A hash is a one-way representation of a password and does not directly reveal it; it must be cracked using tools and wordlists.
2.Weak passwords can be recovered quickly through dictionary attacks regardless of whether the tool is local or online.
3.Local tools like John the Ripper keep data private, while online tools are faster to use but involve sharing the hash with a third-party server.
4.Strong, unique passwords and modern hashing algorithms make cracking significantly harder.

<br>
<div align="center">


**Ethical Note**

</div>

This project was carried out only on a file created for testing purposes, strictly within the scope of this internship, for learning how password hashing and cracking work. The tools and techniques shown here (John the Ripper and Network Walks hash/password cracking tools) should never be used on any file, account, or system without the explicit permission of its owner. Cracking passwords without authorization is illegal and unethical, and this project does not promote or encourage such use.

<br>
<div align="center">


**Author**

</div>

- Name: *Dhanusrika R*
- Internship: Network Walks
- Role:CyberSecurity Intern


