# 📄 Documentation – Zero Trust Network Lab

## 📌 Project Overview

This project demonstrates the implementation of a **Zero Trust Network Architecture** using pfSense firewall in a virtual lab environment.

The objective is to compare:

* Traditional flat network
* Segmented Zero Trust network

---

## 🧱 Lab Environment Setup

### Virtual Machines Used

* Kali Linux (Attacker)
* Ubuntu (Target)
* pfSense Firewall

### Virtualisation Platform

* Oracle VirtualBox

---

## 🌐 Network Configuration

### Traditional Network

* Subnet: 192.168.1.0/24
* All systems in same network
* No firewall restrictions

### Zero Trust Network

* LAN: 192.168.1.0/24 (Kali)
* LAN2: 192.168.2.0/24 (Ubuntu)
* pfSense used for segmentation

---

## 🔐 Firewall Configuration (pfSense)

* LAN → LAN2 traffic blocked
* Only controlled communication allowed
* Rules applied on incoming interface

This ensures that:

* No direct communication between subnets
* All traffic is inspected and controlled

---

## 🧪 Testing Methodology

The following tests were performed:

### 1. Ping Test

* Used to check connectivity between systems

### 2. Nmap Scan

* Used to identify open ports and services

### 3. SSH Access Test

* Used to attempt remote login to target system

---

## 📊 Results Summary

### Traditional Network

* Ping: Successful
* Nmap: Open ports visible
* SSH: Access allowed

### Zero Trust Network

* Ping: Blocked
* Nmap: Ports filtered
* SSH: Access denied

---

## 🔍 Security Analysis

The Zero Trust model successfully:

* Reduces network visibility
* Prevents unauthorised access
* Blocks lateral movement

This demonstrates the importance of segmentation and strict access control.

---

## ⚠️ Limitations

* Small-scale virtual environment
* Limited attack simulations
* Does not represent full enterprise complexity

---

## 🎯 Conclusion

The implementation confirms that Zero Trust significantly improves internal network security compared to traditional flat networks.

---
