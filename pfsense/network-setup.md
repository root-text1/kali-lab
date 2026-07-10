pfSense Network Setup
Objective
Configure pfSense as the core router/firewall for the lab.

1. WAN Configuration
WAN is bridged to your physical network.

Settings:
-DHCP enabled
-Outbound NAT enabled
-Firewall rules allow LAN → WAN

2. LAN Configuration
LAN is the internal lab network.

Settings:
-LAN IP: 10.0.0.1/24
-DHCP enabled
-DNS Resolver enabled
-Firewall rules allow LAN → ANY

3. DHCP Server
Enable DHCP:
Range: 10.0.0.100 – 10.0.0.200
DNS: 10.0.0.1
Gateway: 10.0.0.1

4. DNS Resolver
Enable:
-DNS Resolver
-DNS Forwarding
-Host overrides (optional)

5. Default Gateway
pfSense automatically becomes the gateway for all VMs:

-With Gateway: 10.0.0.1
