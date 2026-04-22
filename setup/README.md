# Setup Guide

## Requirements
- VirtualBox
- pfSense ISO
- Kali Linux ISO
- Ubuntu ISO

---

## Step 1: Create Virtual Machines
- Create 3 VMs:
  - Kali Linux
  - Ubuntu
  - pfSense

---

## Step 2: Configure Networks
- Adapter 1: Internal Network (LAN)
- Adapter 2: Internal Network (LAN2 for pfSense)

---

## Step 3: Assign IP Addresses

### Kali (LAN)
- IP: 192.168.1.100
- Gateway: 192.168.1.1

### Ubuntu (LAN2)
- IP: 192.168.2.104
- Gateway: 192.168.2.1

---

## Step 4: Configure pfSense
- LAN: 192.168.1.1
- LAN2: 192.168.2.1

---

## Step 5: Add Firewall Rules
- Block LAN → LAN2
- Allow only required traffic (if needed)

---

## Step 6: Testing
- Ping
- Nmap
- SSH

---

## Outcome
Zero Trust network successfully blocks communication between subnets.
