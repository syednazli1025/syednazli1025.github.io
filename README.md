# syednazli1025.github.io
Following my Cybersecurity Home Lab Adventures!

1. VM ENVIRONMENT SETUP

Objective:
Build an isolated cybersecurity practice environment using virtual machines to safely perform networking, reconnaissance, and security testing.

• Configured VMware Workstation Pro 17 and created a Windows 10 and Kali Linux virtual machine environment.
• Configured VM storage, virtual hardware, VMware Tools, and network adapter settings.
• Established an isolated host-only virtual network (VMnet1)** for communication between the Windows and Kali VMs.
• Troubleshot VM connectivity and configuration issues, including missing VM files and virtual network adapter settings.
• Verified communication between virtual machines using basic network connectivity tests.


2. VM NETWORK CONFIGURATION AND TROUBLESHOOTING

Objective:
Configure and troubleshoot a private virtual network to enable controlled communication between Windows and Kali Linux systems.

• Configured a host-only VMware network using the **192.168.184.0/24** subnet.
• Identified and verified the IP addresses assigned to the Windows and Kali virtual machines.
• Troubleshot connectivity issues involving incorrect IP addressing and unreachable hosts.
• Used **ping/ICMP testing** to verify communication between virtual machines.
• Investigated Windows firewall/network configuration when connectivity tests initially failed.


3. NETWORK DISCOVERY AND PING SWEEP

Objective:
Identify active hosts on a network by performing network discovery from Kali Linux.

• Performed a ping sweep against the isolated virtual network to identify active systems.
• Used IP addressing information to distinguish between the Kali Linux and Windows hosts.
• Analyzed ICMP responses to determine host availability.
• Used network discovery results as a starting point for subsequent reconnaissance and port-scanning activities.
• Practiced performing reconnaissance within an isolated lab environment.


4. NMAP

Objective:
Use Nmap to identify accessible network services and open ports on a target system.

• Performed Nmap scans from Kali Linux against the Windows virtual machine.
• Identified open TCP ports, including port 445 associated with Windows networking.
• Practiced different Nmap scanning techniques, including TCP connection/ACK-based scanning.
• Interpreted scan results to determine which network services were potentially accessible.
• Used discovered ports to guide additional service enumeration.


6. SERVICE ENUMERATION & BANNER GRABBING

Objective:
Identify services running on discovered open ports and collect information about the target system.

• Developed and executed a Python-based port scanner to identify open TCP ports.
• Enhanced the scanner to associate discovered ports with their corresponding service names.
• Practiced connecting to accessible services to retrieve service banners.
• Used banner information to better understand the software/services exposed by the target.
• Compared automated scanning results with manual enumeration techniques.


8. NETCAT

Objective:
Use command-line networking tools to manually interact with services and understand TCP connections.

• Used Netcat (nc) to establish TCP connections to services within the lab environment.
• Practiced manually connecting to discovered ports after performing Nmap reconnaissance.
• Observed how services respond to incoming connections.
• Used command-line networking techniques to complement automated scanning.
• Compared manual enumeration with information obtained through Nmap and the Python scanner.


9. WIRESHARK

Objective:
Capture and analyze network traffic to understand how network communication appears at the packet level.

• Captured traffic generated between the Windows and Kali virtual machines using Wireshark.
• Applied ICMP display filters to isolate ping traffic.
• Examined packet-level information associated with network connectivity tests.
• Identified source and destination IP addresses within captured packets.
• Connected observable packet activity to commands executed from the terminal.
