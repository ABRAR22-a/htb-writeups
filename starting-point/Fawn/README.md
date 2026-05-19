# Fawn Writeup

## Connecting to VPN

I connected to the Hack The Box VPN using OpenVPN.

```bash
sudo openvpn starting_point.ovpn
```

![VPN Connection](screenshots/vpn.png)

---
## Test connection 


```bash
ping  TARGET_IP
```

![ping](screenshots/ping.png)

---

## Enumeration

```bash
nmap --open -sVC -T4 TARGET_IP
```

![Nmap Scan](screenshots/nmap.png)

The scan revealed that port 21 was open.

FTP stands for File Transfer Protocol and is used for file sharing.


## FTP Connect 

```bash
ftp  TARGET_IP
```

![ftp](screenshots/ftp.png)

I logged in as `anonymous` because we did not have valid account credentials.

## Flag


![flag](screenshots/flag.png)
