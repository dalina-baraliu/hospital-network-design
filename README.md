# Hospital Network Design & Implementation

### Cisco Packet Tracer | Network Engineering | Cybersecurity

A comprehensive academic network engineering project focused on designing, configuring, and testing a secure network infrastructure for a simulated two-floor hospital.

## Project Overview

This project models the network infrastructure of a modern hospital, connecting medical, administrative, and technical departments through a centralized architecture.

The network was designed in Cisco Packet Tracer, with emphasis on network segmentation, secure communication, IP addressing, service availability, and connectivity testing.

The project includes a 93-page technical report covering network architecture, equipment selection, configurations, addressing schemes, security controls, and verification.

## Technologies and Concepts

- Cisco Packet Tracer
- VLANs and IEEE 802.1Q Trunking
- Inter-VLAN Routing (Layer 3 Switching)
- IPv4 Addressing and VLSM
- Access Control Lists (ACLs)
- DHCP and DNS
- HTTP, FTP and Email Services
- VoIP
- Wireless Networking
- IoT Device Integration
- Network Troubleshooting

## Network Architecture

The implemented network follows a simplified two-layer hierarchical architecture:

**Core Layer**
- Central Layer 3 switch
- Inter-VLAN routing
- Network traffic management
- ACL-based access restrictions

**Access Layer**
- Departmental switches
- End-user devices
- Medical and IoT devices
- Wireless infrastructure
- IP phones and CCTV devices

The hospital network spans two floors and supports multiple medical and administrative departments.

## Network Segmentation

The network uses 15 VLANs to separate different departments and services.

| VLAN | Department / Service |
|---|---|
| 10 | Administration |
| 15 | Finance |
| 20 | Emergency |
| 30 | ICU |
| 40 | Surgery |
| 50 | Pharmacy |
| 60 | Radiology |
| 70 | IT |
| 80 | Servers |
| 90 | CCTV / Security |
| 100 | Staff Wi-Fi |
| 110 | Guest Wi-Fi |
| 120 | IoT / Life Safety |
| 150 | VoIP |

**Note:** The design includes 14 listed VLAN IDs above plus the remaining VLAN shown in the full addressing documentation; refer to the technical report for the complete addressing plan.

IPv4 subnetting was performed using VLSM to allocate address space according to departmental requirements.

## Network Security

Security was an important consideration in the project.

### Guest Wi-Fi Access Control

An extended ACL named GUEST_RESTRICTION was configured to restrict Guest Wi-Fi access to internal hospital networks.

The ACL was applied inbound to VLAN 110.

Connectivity tests demonstrated that:
- Authorized devices could access permitted internal resources.
- Guest Wi-Fi devices were blocked from accessing the internal web server.

### Network Segmentation

Department-based VLANs separate traffic into logical network segments.

Inter-VLAN communication is handled by the central Layer 3 switch, allowing traffic control through routing and access policies.

## Implemented Network Services

The simulation includes:

- **DHCP:** Automatic assignment of network settings
- **DNS:** Domain-name resolution
- **Web Server:** Internal hospital webpage
- **FTP Server:** File transfer
- **Mail Server:** Email communication
- **IoT Registration Server:** IoT device management
- **VoIP:** Internal IP telephone communication
- **Wireless:** Separate staff and guest networks

## Testing and Verification

Network functionality was evaluated using Cisco Packet Tracer testing tools and device commands.

Documented tests include:

- Ping connectivity between VLANs
- Access to centralized servers
- DHCP and network service verification
- Guest Wi-Fi access restrictions
- Internal VoIP communication
- IoT device connectivity

Testing evidence and configuration screenshots are available in the technical report.

## Repository Structure

```text
Hospital-Network-Design/
├── packet-tracer/
│   └── Hospital-Network.pkt
├── documentation/
│   └── Hospital-Network-Documentation.pdf
├── screenshots/
│   └── network-topology.png
└── README.md
```

## How to Explore the Project

1. Install Cisco Packet Tracer.
2. Download the .pkt simulation file.
3. Open the project in Packet Tracer.
4. Explore the physical and logical network views.
5. Inspect VLANs, device configurations and services.
6. Reproduce connectivity and access-control tests.

For the complete design and configuration explanation, see the PDF report in the documentation folder.

## Documentation

The full 93-page report includes:

- Network requirements and objectives
- Hardware selection and specifications
- Physical and logical topology diagrams
- VLAN and IPv4 addressing tables
- Configuration examples
- Security policies and ACLs
- Network services
- Connectivity and functionality tests

The full technical report is written in Albanian.

## Disclaimer

This is an academic network simulation developed using Cisco Packet Tracer. All hospital systems, addressing information and device credentials are simulated and do not represent a production healthcare network.

## Author

Dalina Baraliu

[LinkedIn](https://www.linkedin.com/in/dalina-baraliu/)