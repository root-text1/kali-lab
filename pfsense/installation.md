pfSense Installation (VMware Workstation)
Overview
This document explains how to install pfSense as a virtual firewall inside VMware Workstation. pfSense will act as the gateway, DHCP server, DNS resolver, and firewall for the Kali + Windows lab.

1. Download pfSense ISO
Download the latest pfSense Community Edition:

https://www.pfsense.org/download/

Choose:
-Architecture: AMD64
-Installer: ISO
-Console: VGA
-Mirror: Any

2. Create pfSense VM in VMware
-Create New Virtual Machine:
-Choose Typical
-Select the pfSense ISO
-OS type: FreeBSD 64‑bit
-Name: pfSense-Firewall
-Disk: 20 GB
-RAM: 2 GB
-CPU: 2 cores

3. Configure Network Adapters
pfSense needs two NICs:

Adapter 1 — WAN
-Mode: Bridged
Purpose: Connects pfSense to your physical network (Internet)

Adapter 2 — LAN
-Mode: Host-only (recommended)
Purpose: Internal lab network for Kali + Windows

4. Install pfSense
Boot the VM and follow the installer:
-Accept defaults
-Install pfSense
-Auto‑partition
-Reboot

5. Assign Interfaces
pfSense will detect two NICs:
WAN: vmx0
LAN: vmx1

Confirm the interfaces:
WAN: vmx0
LAN: vmx1

6. pfSense LAN IP
Set LAN IP:10.0.0.1
-Subnet: 255.255.255.0
-DHCP: Yes
-Range: 10.0.0.100 – 10.0.0.200

7. Access pfSense Web GUI
From Windows or Kali: https://10.0.0.1

Login:
Username: admin
Password: pfsense (you can select what ever password you like, but make it simplex)
