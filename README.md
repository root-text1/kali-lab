# kali-lab
Kali Lab – Web Server, Mail Server & Networking Project
A complete, fully documented Linux administration lab built on Kali Linux and VMware Workstation, demonstrating practical skills in:
Linux system administration
Apache web server configuration
Postfix + Dovecot mail server setup
VMware bridged networking
IMAP/SMTP testing
Git/GitHub workflow
Technical documentation
Troubleshooting

This project serves as a professional reference and portfolio piece for system administration, cybersecurity, and IT support roles.

- Project Overview
This lab simulates a small enterprise environment using virtual machines:
--Kali Linux Server (10.0.0.151)
Apache Web Server
Postfix SMTP Server
Dovecot IMAP/POP3 Server
Git/GitHub integration
System administration tasks

--Windows 11 Client (10.0.0.175)
Web access
Email client (Thunderbird)
Network testing tools

--VMware Bridged Network
Realistic LAN simulation
Direct communication between VMs
Internet access for updates

This project includes screenshots, configuration files, and step‑by‑step documentation for every component.

- Network Architecture
                   ┌──────────────────────────┐
                   │   Windows 11 Client       │
                   │     IP: 10.0.0.175        │
                   │  - Browser                │
                   │  - Thunderbird (IMAP/SMTP)│
                   └──────────────┬───────────┘
                                  │
                        VMware Bridged Network
                                  │
                   ┌──────────────┴───────────┐
                   │     Kali Linux Server     │
                   │       IP: 10.0.0.151      │
                   │  - Apache Web Server      │
                   │  - Postfix SMTP           │
                   │  - Dovecot IMAP/POP3      │
                   │  - Git/GitHub tools       │
                   └──────────────────────────┘
📁 Repository Structure
kali-lab/
│
├── README.md
│
├── webserver/
│   ├── apache-installation.md
│   ├── apache-config.md
│   ├── troubleshooting.md
│   └── screenshots/
│
├── mailserver/
│   ├── postfix-installation.md
│   ├── dovecot-config.md
│   ├── smtp-imap-tests.md
│   ├── troubleshooting.md
│   └── screenshots/
│
├── network/
│   ├── vmware-bridged.md
│   ├── ip-configuration.md
│   ├── connectivity-tests.md
│   └── screenshots/
│
└── github/
    ├── git-setup.md
    ├── ssh-keys.md
    ├── workflow.md
    └── screenshots/
Each folder contains step‑by‑step instructions, commands, and screenshots documenting the entire configuration process.

🛠 Technologies Used
Kali Linux
VMware Workstation
Apache2
Postfix
Dovecot
Thunderbird (Windows 11)
Git & GitHub
Telnet / Curl / Netcat
Linux CLI tools

🔧 Key Configurations
--Apache Web Server
Installation
Service management
Document root configuration
Testing from Windows
Logs & troubleshooting

--Postfix Mail Server
Internet Site configuration
SMTP testing
Authentication setup
Integration with Dovecot

--Dovecot IMAP/POP3
IMAP/POP3 protocols
Authentication using system users
Service configuration
Telnet testing

--Networking
VMware bridged mode
IP addressing
Ping tests
Connectivity verification

--GitHub Integration
SSH key generation
Git configuration
Cloning & pushing
Repository organization

📸 Screenshots
All screenshots are included in their respective folders:
Web server setup > screenshots
Mail server configuration > screenshots
Network tests > screenshots
GitHub workflow > screenshots

🎯 Skills Demonstrated
This project highlights real-world IT skills such as (and not limited to):
Linux administration
Service configuration
Email protocols (SMTP, IMAP, POP3)
Network troubleshooting
Virtualization
Git/GitHub workflow
Documentation & organization
Problem-solving

These are core competencies for:
System Administrator
IT Support Technician
SOC Analyst
DevOps Junior
Cybersecurity Analyst

🚀 How to Reproduce This Lab :
Install VMware Workstation
Create two VMs: Kali Linux & Windows 11
Configure bridged networking
Install Apache on Kali
Install Postfix + Dovecot
Test IMAP/SMTP from Windows
Configure Git & GitHub
Document everything
Push to GitHub
Full instructions are included in the repository.

📬 Contact
If you want to discuss this project or similar work, feel free to reach out through GitHub or contact me at ttextone@gmail.com
