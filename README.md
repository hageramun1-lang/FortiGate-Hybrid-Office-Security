# FortiGate Hybrid Office Security

## Project Overview

This project demonstrates how to secure a hybrid office network using FortiGate Firewall. The network is divided into three departments: Management, Human Resources (HR), and Developers. Each department has its own security policies and access permissions to ensure a secure and organized network environment.

---

## Objectives

- Design a secure office network using FortiGate.
- Configure separate network segments for Management, HR, and Developers.
- Create Firewall Policies for each department.
- Apply Security Profiles to control network traffic.
- Restrict unauthorized applications and websites.
- Monitor network traffic using FortiGate logs.

---

## Topology

The network consists of:

- FortiGate VM
- Management PC
- HR PC
- Developer PC
- WAN Connection

Each department is connected through a separate interface and protected by dedicated Firewall Policies.

---

## Network Configuration

The following configurations were implemented:

- Interface Configuration
- VMware Network Adapters
- Zones Configuration
- IP Address Assignment
- Static Routing
- NAT Configuration

---

## Firewall Policies

Three Firewall Policies were created:

### Management-to-Internet
- Full Internet access for network administrators.

### HR-to-Internet
- Internet access with restricted applications and websites.
- Application Control applied.
- Web Filter applied.

### DEV-to-Internet
- Internet access for developers.
- Application Control applied.
- Web Filter applied.
- Development resources are allowed according to the security policy.

---

## Security Profiles

The following Security Profiles were configured:

- Application Control
- Web Filter
- SSL Inspection (Certificate Inspection)
- Flow-based Inspection

Different security profiles were assigned based on each department's requirements.

---

## Testing

The project was tested by:

- Verifying Internet connectivity.
- Testing Firewall Policies.
- Monitoring FortiGate Logs.
- Testing blocked and allowed applications.
- Validating Security Profile functionality.

---

## Conclusion

This project demonstrates how FortiGate can be used to secure a hybrid office environment by implementing network segmentation, Firewall Policies, and Security Profiles. It provides a practical example of enterprise network security using FortiOS.

---

## Technologies Used

- FortiGate VM
- FortiOS 7.x
- VMware Workstation
- Windows 10
- Application Control
- Web Filter
- Firewall Policies
- NAT
- VLANs
- Network Zones

---

## Repository Structure

```
FortiGate-Hybrid-Office-Security
│
├── topology
├── Policies
├── HR-Security-Profile
├── HR-Policy-Testing
├── DEV-Security-Profile
├── DEV-Policy-Testing
├── Primal-Configurations
└── README.md
```

## Author

**Hager Amun**
