pfSense Testing & Validation

1. Ping pfSense from Kali
Cmd
ping 10.0.0.1

2. Ping pfSense from Windows
Cmd
ping 10.0.0.1

3. Test Internet from Kali
Cmd
ping google.com

4. Test Internet from Windows
Cmd
ping google.com

5. Access pfSense Web GUI
From browser: https://10.0.0.1

6. Verify DHCP
On Kali:
Cmd
ip addr

On Windows:
Cmd
ipconfig

Expected:
IP in 10.0.0.x
Gateway: 10.0.0.1
DNS: 10.0.0.1

7. Verify Firewall Rules
Navigate:
Cmd
Firewall → Rules → LAN

Ensure:
LAN → ANY allowed
WAN inbound blocked

8. Verify NAT
Navigate:
Cmd
Firewall → NAT → Outbound

Ensure:
Automatic NAT enabled
