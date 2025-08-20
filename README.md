# Linux Network Router Lab

A practical implementation of a software-based router on a Linux Ubuntu Server. This project demonstrates core networking concepts including DHCP, static IP assignment, NAT, and firewall configuration in a virtualized environment.

## 📋 Features

- **DHCP Server:** Automatically assigns IP addresses to clients (range: 192.168.10.100-200)
- **Static IP Configuration:** Router interface configured at 192.168.10.1/24
- **IP Forwarding:** Enabled kernel-level routing between networks
- **Firewall Rules:** Configured iptables for NAT (MASQUERADE) and traffic filtering
- **Virtualization:** Built using OrbStack on macOS

## 🛠️ Technologies Used

- **Operating System:** Ubuntu Server 22.04 LTS
- **Networking:** DHCP (isc-dhcp-server), iptables, Netplan
- **Virtualization:** OrbStack
- **Protocols:** TCP/IP, NAT, DHCP

## 🚀 Configuration Highlights

Key configuration files and commands:

- Netplan config: `/etc/netplan/50-cloud-init.yaml`
- DHCP config: `/etc/dhcp/dhcpd.conf`
- Enabled IP forwarding: `net.ipv4.ip_forward=1`
- iptables NAT rule: `iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE`

## 📸 Project Evidence

<img width="1369" height="327" alt="ip-config" src="https://github.com/user-attachments/assets/93875e1f-1860-43f0-9a44-f62a673e6cb7" />

*Output of `ip addr show` showing successful static IP assignment*

<img width="1440" height="667" alt="dhcp-status png" src="https://github.com/user-attachments/assets/925310f0-d154-40fc-9da1-4901ac46573b" />

*DHCP server running actively and listening on the network interface*

## 🎯 Purpose

This project was developed to gain practical experience in:
- Linux system administration
- Network infrastructure design
- DHCP and NAT implementation
- Firewall configuration
- Virtualization technologies




## 👨‍💻 Author

Rahkhuo Edward
- rahkhuoedward07@gmail.com
