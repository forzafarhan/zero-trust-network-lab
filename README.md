# Zero Trust Network Lab

##  Project Overview

This project demonstrates the implementation and evaluation of a Zero Trust network model compared to a traditional flat network.

The lab environment was created using:
- pfSense (Firewall)
- Kali Linux (Attacker machine)
- Ubuntu (Target machine)
- VirtualBox

The aim of this project is to show how network segmentation improves security by restricting unauthorised access and reducing attack surface.

---

##  Network Architecture

### Traditional Network
- All devices in same subnet (192.168.1.0/24)
- No firewall restrictions
- Full communication allowed

### Zero Trust Network
- Segmented network:
  - LAN → 192.168.1.0/24 (Kali)
  - LAN2 → 192.168.2.0/24 (Ubuntu)
- pfSense firewall controls traffic
- Communication restricted

---

##  Security Implementation

- Firewall rules created in pfSense
- Traffic blocked between subnets
- Only controlled/required access allowed
- Zero Trust principle applied: **never trust, always verify**

---

##  Testing Performed

The following tests were conducted:

- Ping Test (Connectivity)
- Nmap Scan (Reconnaissance)
- SSH Access Test

---

##  Results Summary

| Test  | Traditional Network | Zero Trust Network |
|------|-------------------|------------------|
| Ping | Successful | Blocked |
| Nmap | Open ports visible | Ports filtered |
| SSH  | Accessible | Blocked |

---

## 🎥 Screencast Demonstration

https://roehamptonprod-my.sharepoint.com/:v:/g/personal/mohammem83_roehampton_ac_uk/IQB-QO5JPJPJQLrX8zUJ8uNPARDlHJRFO2hsNhQAAldGwyQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=naLhJw


https://roehamptonprod-my.sharepoint.com/:v:/g/personal/mohammem83_roehampton_ac_uk/IQA2ly3Oi6_XQqp37Ge6anxZAbHKMCLY5nB_YAU8kVzRqV0?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=KnarzS


https://roehamptonprod-my.sharepoint.com/:v:/g/personal/mohammem83_roehampton_ac_uk/IQCKNMVZbQtOTq7mc1O8HKBpAYexs2L_eiWHdrkSt-3Vf1I?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=cVJ7Mp


This video shows:
- Full network setup
- Attack simulations
- Firewall configuration
- Comparison results

---

##  Repository Structure

- `docs/` → Documentation and explanation
- `screenshots/` → All experiment screenshots
- `setup/` → Configuration steps
- `RESULTS/` → Testing outputs

---

##  Key Learning

This project shows that:

- Flat networks are vulnerable to internal attacks
- Network segmentation reduces visibility
- Firewall rules prevent unauthorised access
- Zero Trust improves internal security significantly

---

## 📌 Author
Moinuddin farhan Mohammed
MSc Computing Dissertation  
University of Roehampton  
