pfSense DHCP Configuration
1. Enable DHCP
Navigate:
Services → DHCP Server → LAN
Enable DHCP.

2. Configure DHCP Range
Recommended:
10.0.0.100 – 10.0.0.200

3. Add Static Mappings (Optional)
Example:
Device	MAC Address	IP
Kali	xx:xx:xx:xx	10.0.0.151
Win11	xx:xx:xx:xx	10.0.0.175

4. DNS Settings
Set DNS server: 10.0.0.1

5. Gateway
Set gateway:10.0.0.1
