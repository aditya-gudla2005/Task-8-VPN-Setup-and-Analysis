# Task-8-VPN-Setup-and-Analysis

## Objective:
Demonstrate how VPNs secure internet connections and mask IP addresses by setting up a secure tunnel.

## VPN Used:
- **Hack The Box (HTB) VPN**
- OpenVPN configuration (`.ovpn`) on Kali Linux

## Steps Followed:

1. Downloaded `.ovpn` file from HTB Labs
2. Connected using:
   ```bash
   sudo openvpn ~/Downloads/htb.ovpn
3. VPN assigned internal IP to tun0: 10.23.134.170

4. Verified encryption and IP change using ip a and system logs

5. Disconnected using Ctrl+C after testing routes and connectivity

## VPN Benefits:
1)Encrypts all traffic between user and HTB servers
2)Masks real IP address from the lab environment
3)Prevents data leakage in multi-user lab setups
4)Enhances safety during penetration testing or CTFs

## Limitations:
1) Only routes traffic to lab systems (not full internet VPN)
2) May not hide IP for browser activity
3) Slight decrease in network speed due to encryption

## Screenshots:
-> vpn_on.png: Terminal showing Network interface tun0 IP details after vpn connection

-> vpn_screenshot_2.png: Terminal showing Network interface after turning off the vpn connection

## Outcome:
Successfully connected to HTB VPN, verified IP tunneling, and understood the encryption and routing involved in secure VPN communication.
