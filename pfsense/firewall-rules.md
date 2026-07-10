pfSense Firewall Rules
1. LAN Rules
Default rule:

Cmd
LAN → ANY (Allow)
This allows Kali + Windows to reach WAN and each other.

2. WAN Rules
Default:

cmd
Block all inbound WAN traffic
This protects the lab.

3. Optional Rules
Allow ICMP (Ping)

cmd
LAN → WAN → ICMP → Allow
Allow Web GUI from LAN

cmd
LAN → 10.0.0.1 → HTTPS → Allow
Block LAN → LAN (segmentation)

cmd
LAN → LAN → Block
