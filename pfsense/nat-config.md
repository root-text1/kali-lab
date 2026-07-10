pfSense NAT Configuration
1. Outbound NAT
Use Automatic Outbound NAT (default).

This allows LAN devices to reach the Internet.

2. Port Forwarding (Optional)
Example: Forward HTTP to Kali:

Cmd
WAN → 80 → 10.0.0.151
Example: Forward SMTP:

Cmd
WAN → 25 → 10.0.0.151

3. NAT Reflection
Enable if you want internal devices to reach WAN‑side services.
