# NetPractice

<div align="right">

[![GitHub stars](https://img.shields.io/github/stars/OliverKingz/NetPractice?color=brightgreen)]()  
 [![Visits Badge](https://badges.pufler.dev/visits/OliverKingz/NetPractice)]()  
 [![Created Badge](https://badges.pufler.dev/created/OliverKingz/NetPractice)]()  
 [![Updated Badge](https://badges.pufler.dev/updated/OliverKingz/NetPractice)]()

</div>

[**42 Cursus Project**] NetPractice is practical networking exercise to configure small-scale networks using TCP/IP addressing principles. Solve 10 simulated network problems to ensure proper functionality.

**Keywords**

- **TCP/IP Addressing**
- **Network Configuration**
- **Subnetting**
- **Routers**
- **Simulated Networks**

<div align="right">

Made by: [![Contributors Display](https://badges.pufler.dev/contributors/OliverKingz/NetPractice?size=30&padding=5&perRow=10&bots=true)](https://github.com/OliverKingz)

</div>

---

## Index

- [Overview](#overview)
- [Features](#features)
- [What I Learned](#what-i-learned)
- [Submission](#submission)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

---

## Overview

NetPractice is a hands-on project designed to teach the fundamentals of networking, focusing on TCP/IP addressing and network device configuration. Through a browser-based interface, users solve 10 progressively challenging levels by correcting misconfigured networks. The project emphasizes practical understanding of routers, subnets, and IP allocation.

**Key Tools**:

- Web-based training interface (`index.html`).
- Manual configuration of IP addresses, subnets, and gateways.

---

## Features

- **10 Simulated Levels**: Each level presents a unique network diagram with specific issues to resolve.
- **Interactive Interface**: Real-time feedback via logs and validation checks.
- **Config Export**: Save configurations for submission using the `[Get my config]` button.
- **Defense Mode**: Complete 3 random levels under time constraints during evaluation.

---

## Networking Basics (IPv4)

This project focuses on IPv4, which uses 32-bit addresses divided into four 8-bit sections (like 192.168.100.1). Each section can range from 0 to 255.

### Network Masks

A network mask (or subnet mask) defines which IP addresses belong to the same subnet (network). It's also a 32-bit number, but its binary representation must have all 1s on the left followed by all 0s on the right (e.g., 255.255.255.0 is valid, 255.255.128.128 is not).

Masks can be written in "dot-decimal notation" (e.g., 255.255.255.0) or CIDR notation (e.g., /24). A smaller CIDR number (like /16) means a larger subnet with more usable IP addresses.

**Important:** Each subnet reserves two IP addresses:

- The network address (the first address in the range)
- The broadcast address (the last address in the range)  
  These two addresses cannot be assigned to devices.

#### Subnetting Reference Table

<div align="center">

| CIDR |   Dot-decimal   | Nº of IP-addresses/subnet | Usable IP's/subnet | Number of subnets |
| :--: | :-------------: | :-----------------------: | :----------------: | :---------------: |
| /32  | 255.255.255.255 |             1             |         0          |        256        |
| /31  | 255.255.255.254 |             2             |         0          |        128        |
| /30  | 255.255.255.252 |             4             |         2          |        64         |
| /29  | 255.255.255.248 |             8             |         6          |        32         |
| /28  | 255.255.255.240 |            16             |         14         |        16         |
| /27  | 255.255.255.224 |            32             |         30         |         8         |
| /26  | 255.255.255.192 |            64             |         62         |         4         |
| /25  | 255.255.255.128 |            128            |        126         |         2         |
| /24  |  255.255.255.0  |            256            |        254         |         1         |
| /23  |  255.255.254.0  |            512            |        510         |        N/A        |
| /22  |  255.255.252.0  |           1024            |        1022        |        N/A        |
| /21  |  255.255.248.0  |           2048            |        2046        |        N/A        |
| /20  |  255.255.240.0  |           4096            |        4094        |        N/A        |
| /19  |  255.255.224.0  |           8192            |        8190        |        N/A        |
| /18  |  255.255.192.0  |           16384           |       16382        |        N/A        |

<details>
  <summary>Show more of the table</summary>

| CIDR |  Dot-decimal  | Nº of IP-addresses/subnet | Usable IP's/subnet | Number of subnets |
| :--: | :-----------: | :-----------------------: | :----------------: | :---------------: |
| /17  | 255.255.128.0 |           32768           |       32766        |        N/A        |
| /16  |  255.255.0.0  |           65536           |       65534        |        N/A        |
| /15  |  255.254.0.0  |          131072           |       131070       |        N/A        |
| /14  |  255.252.0.0  |          262144           |       262142       |        N/A        |
| /13  |  255.248.0.0  |          524288           |       524286       |        N/A        |
| /12  |  255.240.0.0  |          1048576          |      1048574       |        N/A        |
| /11  |  255.224.0.0  |          2097152          |      2097150       |        N/A        |
| /10  |  255.192.0.0  |          4194304          |      4194302       |        N/A        |
|  /9  |  255.128.0.0  |          8388608          |      8388606       |        N/A        |
|  /8  |   255.0.0.0   |         16777216          |      16777214      |        N/A        |
|  /7  |   254.0.0.0   |         33554432          |      33554430      |        N/A        |
|  /6  |   252.0.0.0   |         67108864          |      67108862      |        N/A        |
|  /5  |   248.0.0.0   |         134217728         |     134217726      |        N/A        |
|  /4  |   240.0.0.0   |         268435456         |     268435454      |        N/A        |
|  /3  |   224.0.0.0   |         536870912         |     536870910      |        N/A        |
|  /2  |   192.0.0.0   |        1073741824         |     1073741822     |        N/A        |
|  /1  |   128.0.0.0   |        2147483648         |     2147483646     |        N/A        |
|  /0  |    0.0.0.0    |        4294967296         |     4294967294     |        N/A        |

</details>
</div>

### Special IP Ranges

Certain IP address ranges are reserved for specific purposes:

- **Private Networks:** Used within local networks and not routable on the global internet. Important for security and internal communication. Internet routers ignore these addresses, preventing external access.
  - 10.0.0.0 – 10.255.255.255
  - 172.16.0.0 – 172.31.255.255
  - 192.168.0.0 – 192.168.255.255
- **Loopback Addresses:** Used for testing and internal communication within a single device.
  - 127.0.0.0 – 127.255.255.255

### Network Devices & Routing

- **Switches:** Connect multiple devices within the same network, distributing data packets to their intended recipients.
- **Routers:** Essential for communication between different networks. A router has multiple interfaces, each connecting to a different network.
- **Routing Table:** Each router maintains a routing table that tells it the paths to various networks. It consists of:
  - **Destination:** The target network address (e.g., 190.3.2.252/30) or 0.0.0.0/0 (for a default route to any unknown network).
  - **Next Hop:** The IP address of the next router in the path to the destination network.

### How Networks Work Together

To send data between IP addresses:

- **Same Network:** Devices must be in the same network. You determine if devices are in the same network by performing a bit-by-bit AND operation between their IP address and their subnet mask. If the resulting "network address" is identical for two devices, they are in the same network.  
  Example: 192.168.100.1 AND 255.255.255.0 results in 192.168.100.0 (the network address).
- **Different Networks:** If devices are in different networks, they must be connected via one or more routers. Routers use their routing tables to forward packets from one network to another until they reach the destination network.

Understanding these fundamentals of IP addresses, masks, and routing is crucial for designing and troubleshooting networks.

---

## What I Learned

- **TCP/IP Addressing**: Mastered subnetting and gateway configuration.
- **Problem-Solving**: Diagnosed network issues using logical deduction.
- **Precision**: Small errors (e.g., incorrect subnet masks) break entire networks.
- **Understanding of Network Devices**: Gained knowledge about various network devices (routers, and its routing table, and switches) and their roles in a network.

---

## Solutions

The solutions for each level are provided below. Each solution is a screenshot of the completed network configuration for that level.
The solutions are organized by level, with each level's solution displayed in a collapsible section for easy navigation.

<details>
  <summary><strong>Show Solutions</strong></summary>

  <details>
    <summary><strong>Level 1</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_01.png" alt="Level 1 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 2</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_02.png" alt="Level 2 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 3</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_03.png" alt="Level 3 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 4</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_04.png" alt="Level 4 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 5</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_05.png" alt="Level 5 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 6</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_06.png" alt="Level 6 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 7</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_07.png" alt="Level 7 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 8</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_08.png" alt="Level 8 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 9</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_09.png" alt="Level 9 Solution" width="600"/>
    </p>
  </details>

  <details>
    <summary><strong>Level 10</strong></summary>
    <p align="center">
      <img src="solutions/NetPractice_10.png" alt="Level 10 Solution" width="600"/>
    </p>
  </details>

</details>

---

## Author

<div align="center">

| **Name**               | **GitHub Profile**                            | **42 Login** |
| ---------------------- | --------------------------------------------- | ------------ |
| **Oliver King Zamora** | [OliverKingz](https://github.com/OliverKingz) | **ozamora-** |

</div>

---

## Acknowledgments

- **42 Network**: For the simulated training environment.
- **Peers**: Collaborative debugging and subnetting tips.

---
