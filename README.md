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
- [How to Use](#how-to-use)
  - [Example Usage](#example-usage)
  - [Error Handling](#error-handling)
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

## How to Use

### Setup

1. Download and extract the project files.
2. Open `index.html` in a web browser.
3. Enter your 42 intranet login (or leave empty for defense mode).

### Steps

1. **Select a Level**: Choose from 10 available levels.
2. **Configure the Network**: Fill in unshaded fields (e.g., IP addresses, subnet masks).
3. **Validate**: Click `[Check again]` to test your solution.
4. **Export**: Use `[Get my config]` to save your configuration for submission.
5. **Proceed**: Click `[Next level]` after successful completion.

### Example Usage

| **Action**                            | **Description**                            | **Expected Outcome**                        |
| ------------------------------------- | ------------------------------------------ | ------------------------------------------- |
| Set `192.168.1.1` as gateway          | Configures the default route for a subnet. | Devices can communicate outside the subnet. |
| Adjust subnet mask to `255.255.255.0` | Defines a Class C network.                 | Correctly partitions IP addresses.          |

### Error Handling

- **Invalid IP**: Logs display "Error: Invalid IP range."
- **Misconfigured Router**: "No route to host" error in logs.

---

## What I Learned

- **TCP/IP Addressing**: Mastered subnetting and gateway configuration.
- **Problem-Solving**: Diagnosed network issues using logical deduction.
- **Precision**: Small errors (e.g., incorrect subnet masks) break entire networks.

---

## Submission

- Submit **10 configuration files** (1 per level) to your Git repository.
- Files must be exported via `[Get my config]` and placed at the root of the repo.
- **Defense**: Complete 3 random levels in 15 minutes without external tools.

> **NOTE**: Ensure your login is entered in the interface to link configurations to your profile.

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
- **RFC 791**: Reference for IP addressing standards.

---

## Subnetting Reference Table

| CIDR |   Dot-decimal   | Nº of IP-addresses / subnet | Usable IP-addresses / subnet | Number of subnets |
| :--: | :-------------: | :-------------------------: | :--------------------------: | :---------------: |
| /32  | 255.255.255.255 |              1              |              0               |        256        |
| /31  | 255.255.255.254 |              2              |              0               |        128        |
| /30  | 255.255.255.252 |              4              |              2               |        64         |
| /29  | 255.255.255.248 |              8              |              6               |        32         |
| /28  | 255.255.255.240 |             16              |              14              |        16         |
| /27  | 255.255.255.224 |             32              |              30              |         8         |
| /26  | 255.255.255.192 |             64              |              62              |         4         |
| /25  | 255.255.255.128 |             128             |             126              |         2         |
| /24  |  255.255.255.0  |             256             |             254              |         1         |
| /23  |  255.255.254.0  |             512             |             510              |        N/A        |
| /22  |  255.255.252.0  |            1024             |             1022             |        N/A        |
| /21  |  255.255.248.0  |            2048             |             2046             |        N/A        |
| /20  |  255.255.240.0  |            4096             |             4094             |        N/A        |
| /19  |  255.255.224.0  |            8192             |             8190             |        N/A        |
| /18  |  255.255.192.0  |            16384            |            16382             |        N/A        |
| /17  |  255.255.128.0  |            32768            |            32766             |        N/A        |
| /16  |   255.255.0.0   |            65536            |            65534             |        N/A        |
| /15  |   255.254.0.0   |           131072            |            131070            |        N/A        |
| /14  |   255.252.0.0   |           262144            |            262142            |        N/A        |
| /13  |   255.248.0.0   |           524288            |            524286            |        N/A        |
| /12  |   255.240.0.0   |           1048576           |           1048574            |        N/A        |
| /11  |   255.224.0.0   |           2097152           |           2097150            |        N/A        |
| /10  |   255.192.0.0   |           4194304           |           4194302            |        N/A        |
|  /9  |   255.128.0.0   |           8388608           |           8388606            |        N/A        |
|  /8  |    255.0.0.0    |          16777216           |           16777214           |        N/A        |
|  /7  |    254.0.0.0    |          33554432           |           33554430           |        N/A        |
|  /6  |    252.0.0.0    |          67108864           |           67108862           |        N/A        |
|  /5  |    248.0.0.0    |          134217728          |          134217726           |        N/A        |
|  /4  |    240.0.0.0    |          268435456          |          268435454           |        N/A        |
|  /3  |    224.0.0.0    |          536870912          |          536870910           |        N/A        |
|  /2  |    192.0.0.0    |         1073741824          |          1073741822          |        N/A        |
|  /1  |    128.0.0.0    |         2147483648          |          2147483646          |        N/A        |
|  /0  |     0.0.0.0     |         4294967296          |          4294967294          |        N/A        |
