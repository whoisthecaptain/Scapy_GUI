# Scapy_GUI
Universal Scapy Packet Builder GUI is a Python/Tkinter graphical tool for building, previewing, saving, and exporting Scapy packets.


# Universal Scapy Packet Builder GUI

## Overview

Universal Scapy Packet Builder GUI is a Python-based graphical interface for crafting Scapy packets. It allows users to build packet layer stacks, edit packet fields, preview packet structure, save packets to PCAP, export Python Scapy scripts, and send packets in an authorized lab environment.

This tool is intended for cybersecurity labs, protocol analysis, Wireshark practice, and learning how network packets are built.

## Features

- Graphical packet builder using Tkinter
- Dynamic Scapy layer discovery
- Layer stack editor
- Friendly field descriptions for common packet fields
- Built-in packet templates
- Raw Scapy expression mode
- PCAP export
- Python script export
- Wireshark launch support
- Interface detection
- Wireless monitor-mode detection
- Optional managed-to-monitor mode prompt
- Authorized-lab checkbox before live packet sending
- Send Packet Again button
- Help Manual tab
- Scapy Layer Browser tab
- Live-send block for deauthentication and disassociation packets

## Built-In Packet Templates

The GUI includes templates for:

- 802.11 ICMP payload packet
- Ethernet ICMP echo request
- ARP request
- ARP reply
- TCP SYN
- UDP payload
- DNS A record query
- DNS A record response
- DNS TXT query
- DHCP Discover
- 802.11 beacon
- 802.11 directed probe request
- 802.11 RTS
- 802.11 deauthentication packet for PCAP-only analysis

## Safety Controls

This tool includes built-in safety controls.

Live packet sending requires the user to check:

```text
I confirm I am in an authorized lab environment.
