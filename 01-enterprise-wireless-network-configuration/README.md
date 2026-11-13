# Enterprise Wireless Network Configuration Using Cisco Packet Tracer

## 1. Project Overview

This project involved designing and configuring a centrally managed enterprise wireless network using Cisco Packet Tracer.

The network supports four departments: IT, HR, Finance and Management. Each department has a dedicated Wireless LAN (WLAN), with a unique Service Set Identifier (SSID) and password, mapped to a separate VLAN.

A Wireless LAN Controller (WLC) centrally manages four lightweight Access Points (LAPs), providing wireless connectivity to clients across the different departments.

The project also involved configuring DHCP and DNS services, assigning default gateways, and testing connectivity between devices across different VLANs.

## 2. Project Objectives

- Configure a Wireless LAN Controller to manage multiple lightweight Access Points.
- Create separate WLANs for different departments.
- Map each WLAN to its corresponding VLAN.
- Configure wireless security using departmental SSIDs and passwords.
- Provide automatic IP address assignment through DHCP.
- Configure DNS and default gateway services.
- Verify wireless connectivity and inter-VLAN communication.
- Troubleshoot wireless client connectivity issues.

## 3. Tools and Technologies

- Cisco Packet Tracer
- Wireless LAN Controller (WLC)
- Lightweight Access Points (LAPs)
- Virtual Local Area Networks (VLANs)
- Wireless LANs (WLANs) and SSIDs
- Dynamic Host Configuration Protocol (DHCP)
- Domain Name System (DNS)
- Inter-VLAN routing
- Wireless security

## 4. Network Topology

The network consists of 13 devices:

| Device | Quantity |
|---|---:|
| Wireless LAN Controller | 1 |
| Lightweight Access Points | 4 |
| Wireless Tablets | 4 |
| Switch | 1 |
| Router | 1 |
| Server | 1 |
| Management PC | 1 |
| **Total** | **13** |

The network topology diagram is available in the [`topology/`](topology/) directory.

## 5. VLAN and WLAN Configuration

Each department was assigned a dedicated VLAN and WLAN to provide logical network separation.

| Department | VLAN ID |
|---|---:|
| IT | 10 |
| HR | 20 |
| Finance | 30 |
| Management | 50 |

Each WLAN was configured with a unique departmental SSID and password and mapped to its corresponding VLAN through the WLC.

This allowed wireless clients to connect to their respective departmental networks.

## 6. Implementation

### 6.1 Wireless LAN Controller

- Configured the WLC management interface.
- Created four departmental WLANs.
- Assigned a unique SSID to each WLAN.
- Configured wireless security and passwords.
- Mapped each WLAN to its corresponding departmental VLAN.

### 6.2 Access Points

- Connected four lightweight Access Points to the network.
- Joined all four Access Points to the WLC.
- Verified that the WLC successfully managed the connected Access Points.

### 6.3 Wireless Clients

- Connected four tablets to their respective departmental SSIDs.
- Verified that each tablet received an IP address.
- Tested wireless roaming between Access Points while maintaining connectivity to the assigned WLAN.

### 6.4 Network Services

- Configured DHCP on the server to provide automatic IP address assignment.
- Configured DNS services on the server.
- Used the router to provide default gateway services and facilitate inter-VLAN communication.

## 7. Testing and Verification

The following tests were performed to verify the network implementation:

| Test | Result |
|---|---|
| All four APs joined the WLC | Successful |
| Departmental WLANs created | Successful |
| Tablets connected to assigned WLANs | Successful |
| Wireless clients received IP addresses | Successful |
| Wireless roaming between APs | Successful |
| Communication between devices in different VLANs | Successful |

## 8. Troubleshooting

During testing, one wireless client initially failed to obtain an IP address.

After investigating the WLAN configuration, I discovered a typographical error in the WLAN setup.

I corrected the error and repeated the connection test. The client subsequently obtained an IP address successfully.

This experience reinforced the importance of verifying WLAN configuration details when troubleshooting wireless connectivity and DHCP-related issues.

It also highlighted how a small configuration error can affect communication across an otherwise functional network.

## 9. Key Lessons Learned

- A WLC provides centralised management of lightweight Access Points.
- Multiple Access Points can broadcast departmental WLANs.
- WLAN-to-VLAN mapping determines the VLAN associated with wireless client traffic.
- Wireless clients can roam between Access Points while maintaining their WLAN connection.
- DHCP automates IP address assignment, while DNS resolves domain names.
- A router can provide default gateways and facilitate communication between VLANs through inter-VLAN routing.
- Configuration verification and systematic troubleshooting are essential when implementing and maintaining networks.

## 10. Project Files

| Directory | Description |
|---|---|
| `packet-tracer/` | Cisco Packet Tracer project file. |
| `topology/` | Network topology diagram. |
| `screenshots/` | Evidence of configurations and verification tests. |

## 11. Conclusion

This project provided practical experience in configuring a centrally managed enterprise wireless network with departmental WLANs, VLAN segmentation, DHCP, DNS and inter-VLAN communication.

It also provided an opportunity to troubleshoot a configuration error, investigate its cause and verify the effectiveness of the correction through testing.

This project forms part of my ongoing practical work as I strengthen my networking knowledge and prepare for the CCNA certification.
