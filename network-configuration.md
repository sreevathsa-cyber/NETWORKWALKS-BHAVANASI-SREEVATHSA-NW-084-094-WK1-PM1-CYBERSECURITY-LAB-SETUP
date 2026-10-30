# Network Configuration

Record only values observed in VirtualBox and Kali Linux.

| Setting | Observed value |
|---|---|
| VirtualBox network mode | [Fill in] |
| NAT Network name (if used) | [Fill in] |
| Network CIDR | [Fill in] |
| Kali interface name | [Fill in] |
| Kali IP address | [Fill in] |
| Default gateway | [Fill in] |
| DNS resolver | [Fill in] |
| DHCP enabled? | [Yes / No / N/A] |

## Commands used

```bash
ip a
ip route
cat /etc/resolv.conf
```

## Connectivity evidence

```bash
ping -c 4 <gateway-ip>
getent hosts kali.org
```

Paste concise outputs or attach screenshots in `../screenshots/network/`.

**Privacy:** Review screenshots before publishing. Do not expose passwords, tokens, personal files, or unrelated private information.
