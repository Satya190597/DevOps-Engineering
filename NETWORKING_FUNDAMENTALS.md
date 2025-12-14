# Fundamentals of Networking
## Summary
Computer networking involves connecting computing devices to share data and resources. These connections enable communication through wired or wireless mediums using standardized protocols.
## Hardware components of Networking
**Switch**

A network switch is a hardware device that connects multiple devices within a local area network (LAN) by intelligently forwarding data packets based on **MAC addresses**. It operates primarily at **Layer 2** of the OSI model, using a MAC address table to direct traffic only to the intended recipient, unlike hubs that broadcast to all ports.

**Router**

A router is a networking hardware device that forwards data packets between computer networks, connecting **multiple LANs** or **subnetworks** to enable communication across them. It operates at **Layer 3** of the OSI model, using **IP addresses** and **routing tables** to determine the optimal path for data transmission, unlike switches which focus on MAC addresses within a single network.

**Hub**

A network hub is a basic hardware device that connects multiple devices in a local area network (LAN) by broadcasting incoming data packets to all connected ports. It operates at **Layer 1** (Physical layer) of the OSI model, functioning like a multi-port repeater without any intelligence to direct traffic.

**Bridge**

A network bridge connects multiple network segments, such as LANs, to function as a single network while filtering traffic based on MAC addresses. It operates at **Layer 2** (Data Link layer) of the OSI model, reducing collisions by segmenting traffic unlike hubs.

## Difference between MAC Address and IP Address
| Aspect | MAC Address | IP Address |
|--------|-------------|------------|
| **Full Name** | Media Access Control | Internet Protocol |
| **Layer (OSI Model)** | Data Link (Layer 2) | Network (Layer 3) |
| **Format** | 6-byte hexadecimal (e.g AA:BB:CC:DD:EE:FF) | 4-byte IPv4 (e.g 192.168.1.1) or 16-byte IPv6 |
| **Scope** | Local network only | Across networks/internet |
| **Assigned By** | Device manufacturer (NIC) | ISP, DHCP, or admin |
| **Changeable** | Permanent (hardware-burned) | Dynamic, changes per network |
| **Used By** | Switches for local delivery |  Routers for path determination |

## Flow of packets over internet.
> | MY PC | ---> | SWITCH | ---> | ROUTER | ---> | FIRE WALL | ---> | MODEM | ---> | INTERNET |
