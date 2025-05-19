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
| **Action**               | **Description**                                  | **Expected Outcome**                          |  
|--------------------------|--------------------------------------------------|-----------------------------------------------|  
| Set `192.168.1.1` as gateway | Configures the default route for a subnet.     | Devices can communicate outside the subnet.   |  
| Adjust subnet mask to `255.255.255.0` | Defines a Class C network.          | Correctly partitions IP addresses.            |  

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

| **Name**                   | **GitHub Profile**                              | **42 Login** |  
| -------------------------- | ----------------------------------------------- | ------------ |  
| **Oliver King Zamora**              | [OliverKingz](https://github.com/OliverKingz)    | **ozamora-**   |  

</div>

---

## Acknowledgments  
- **42 Network**: For the simulated training environment.  
- **Peers**: Collaborative debugging and subnetting tips.  
- **RFC 791**: Reference for IP addressing standards.  
