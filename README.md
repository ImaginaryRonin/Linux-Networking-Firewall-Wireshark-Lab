# Linux Networking, Firewall, and Wireshark Guide
Create a working Linux network and learn how computers actually communicate with each other. Configure IP addresses and gateways, connect your VM to the host machine, control traffic with firewall rules, test connectivity, and use Wireshark to see the packets moving across the network.

<br>

## Before You Begin
**Difficulty Level:** Beginner to Intermediate

Prior networking experience is **not required**.

#### Before proceeding with this lab, the user should have:
- Basic Windows 11 navigation knowledge
- Administrative access on their host machine
- Access to a trusted home network or isolated lab network
  
<br>
<br>

## Skills Achieved
By completing this lab, the user will:
- Identify and configure Linux network interfaces
- Assign static IPv4 addresses, subnet masks, gateways, and DNS settings
- Understand DHCP, private IP addressing, and basic routing
- Set up VirtualBox Bridged Adapter networking
- Establish and verify bidirectional communication between Windows and Linux
- Diagnose network connectivity using `ping`, `ip`, and `nmcli`
- Manage firewall zones, ports, and ICMP rules using `firewalld`
- Demonstrate the effects of permitting and blocking network traffic
- Capture and analyze ARP, ICMP, TCP, and DNS traffic using Wireshark
- Troubleshoot common Linux networking and firewall problems

<br>
<br>

## Table of Contents

| Section | Purpose |
| --- | --- |
| [Before You Begin](#before-you-begin) | Guide difficulty, prerequisites, and expected starting knowledge. |
| [Skills Achieved](#skills-achieved) | Summary of the technical skills demonstrated. |
| [System Requirements](#system-requirements) | Hardware and software requirements. |
| [Key Terms](#key-terms) | Explanation of important technical terms used. |
| Networking |  |
| [Part 1.1: Identify the Windows Host Network](#part-11-inspect-the-windows-host-network) | Find the Windows host's IPv4 address, subnet mask, default gateway, and active network adapter. |
| [Part 1.2: Set Up VirtualBox Bridged Networking](#part-12-set-up-virtualbox-bridged-networking) | Configure the virtual machine's network adapter to connect to the same local network as the Windows host. |
| [Part 1.3: Examine Linux Network Interfaces and Connections](#part-13-examine-linux-network-interfaces-and-connections) | Identify the CentOS network interface, active NetworkManager connection profile, and existing IP configuration. |
| [Part 1.4: Assign Static IPv4 Addressing](#part-14-assign-static-ipv4-addressing) | Configure a persistent IPv4 address, subnet prefix, default gateway, and DNS settings for the Linux VM. |
| [Part 1.5: Verify Network Connectivity and Routing](#part-15-verify-network-connectivity-and-routing) | Test gateway access, DNS resolution, internet connectivity, and communication between Windows and Linux in both directions. |
| Firewall |  |
| [Part 2.1: Review Linux Firewall Configuration](#part-21-review-linux-firewall-configuration) | Check the status of `firewalld` and identify active firewall zones, allowed services, open ports, and existing rules. |
| [Part 2.2: Block and Restore ICMP (Ping) Traffic](#part-22-block-and-restore-icmp-ping-traffic) | Use firewall rules to block incoming ping requests from Windows, test the results, and restore communication. |
| [Part 2.3: Control TCP Port Access](#part-23-control-tcp-port-access) | Create a temporary HTTP server and test how allowing or blocking a TCP port affects connections from Windows. |
| Wireshark |  |
| [Part 3.1: Install Wireshark on Windows](#part-31-install-wireshark-on-windows) | Install Wireshark and Npcap, then select the correct network adapter to prepare for packet capture. |
| [Part 3.2: Capture Network Traffic](#part-32-capture-network-traffic) | Generate and record ARP, ICMP, TCP, and DNS traffic using the Windows host and Linux VM. |
| [Part 3.3: Analyze Captured Packets](#part-33-analyze-captured-packets) | Examine packet details, identify source and destination addresses, and explain how different protocols handle network communication. |
| [Bonus Steps](#bonus-steps) | Optional functionality, improvements, and/or quality-of-life steps. |
| [Troubleshooting](#troubleshooting) | Common problems and their solutions. |
| [Closing Notes](#closing-notes) | Final summary, applications, and how it supports future IT portfolio projects. |

<br>
<br>

## System Requirements

### Minimum System Requirements
| Component | Minimum Requirement |
| --- | --- |
| Host Operating System | Windows 11 |
| CPU | 64-bit dual-core processor |
| RAM | 8 GB minimum |
| Storage | At least 40 GB of free disk space |
| Internet Connection | Required |


### Software Requirements
| Software | Purpose |
| --- | --- |
| [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads) | Creates, manages, and runs multiple virtual machines. |
| [[CloudOS Stream 9](https://www.centos.org/download/) | Linux operating system used for networking, firewall configuration, and connectivity testing. |

<br>
<br>

## Key Terms

| Term | Meaning |
| --- | --- |
| [Term 1] | [Simple Explanation]. |
| [Term 2] | [Simple Explanation]. |
| [Term 3] | [Simple Explanation]. |
| [Term 4] | [Simple Explanation]. |
| [Term 5] | [Simple Explanation]. |
| [Term 6] | [Simple Explanation]. |

<br>
<br>

# The Guide

## Step 1: [First Major Task]
[Brief explanation of this step and why it matters.]

1.  
2.
3.  <br>

   [Screenshot if necessary] <br>
   [Note if necessary] <br>
   
[Common Error 1: (#common-error-1-)  

<br>
<br>


# Bonus Steps
## Bonus Steps 1: [First Bonus Step]
[Brief explanation of this step and why it matters.]

1.  
2.
3.  <br>

   [Screenshot if necessary] <br>
   [Note if necessary] <br>
   
[Common Error 2: (#common-error-2-)  

<br>
<br>

# Troubleshooting

## Common Error 1: [First Common Error]
[Brief explanation of this step and why it matters.]
[Possible causes.]

To resolve this:

1.  
2.
3.  <br>

   [Screenshot if necessary] <br>
   [Note if necessary] <br>

<br>
<br>

## Common Error 2: [Second Common Error]
[Brief explanation of this step and why it matters.]
[Possible causes.]

To resolve this:

1.  
2.
3.  <br>

   [Screenshot if necessary] <br>
   [Note if necessary] <br>

<br>
<br>


# Closing Notes
[What the reader has successfully built, configured, or accomplished.]

[Explain how this lab can be used in practical situations or expanded through future labs.]

[Close with the usefulness of the skills demonstrated and how this project connects to the rest of the reader's career.]









