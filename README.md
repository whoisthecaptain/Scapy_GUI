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

## Legal and Authorized Use Notice

This tool is provided for educational, research, and authorized lab use only. It is intended to help users understand packet structure, protocol behavior, Wireshark analysis, and Scapy scripting in controlled environments.

By using this tool, you are responsible for ensuring that all activity is permitted by law, policy, and the rules of the network or lab environment you are working in.

## Authorized Environments Only

Only use packet transmission features in environments where you have explicit permission, such as:

- Your own isolated lab network
- A classroom lab environment
- A sanctioned cyber range
- A capture-the-flag or training environment where packet crafting is allowed
- A work environment where you have written authorization to test
- A virtualized lab using local VMs or intentionally isolated interfaces

Do not transmit crafted packets on public networks, production networks, enterprise networks, school networks, government networks, hotel Wi-Fi, coffee shop Wi-Fi, or any network where you do not have clear authorization.

## User Responsibility

The user is fully responsible for how this tool is used. Before sending any packet, confirm that:

- You own or are authorized to use the target network
- You are allowed to generate custom traffic
- The test will not disrupt other users or systems
- The test scope is clearly defined
- The interface and destination are correct
- You understand what the packet is designed to do
- You have permission to capture and inspect the resulting traffic

Accidental misuse can still cause disruption. Always verify packet contents in Wireshark before using any send function.

## No Unauthorized Testing

Do not use this tool for:

- Unauthorized network probing
- Interfering with wireless clients
- Disrupting network availability
- Bypassing access controls
- Impersonating devices on networks you do not own
- Sending traffic to third-party systems without permission
- Testing against public IP addresses without written authorization
- Any activity that violates law, policy, or acceptable use rules

## Wireless Safety Notice

Wireless packet crafting can affect nearby devices if transmitted over the air. Only use wireless transmission features inside an authorized lab environment with approved hardware and clear boundaries.

For 802.11 testing:

- Use monitor mode only when permitted
- Use low-power or isolated lab setups when possible
- Avoid testing near networks or clients outside your scope
- Do not send frames intended to disconnect, disrupt, or degrade other users
- Confirm the correct interface before sending

This GUI blocks live sending of deauthentication and disassociation packets by design. Those packet types are included only for PCAP generation and Wireshark analysis.

## Bluetooth and RF Notice

Bluetooth, BLE, Wi-Fi, and other RF protocols may be regulated depending on your location, hardware, frequency, and test method. Only perform RF testing where permitted and within the rules of your lab, organization, and local law.

## No Warranty

This tool is provided as-is, without warranty of any kind. There is no guarantee that generated packets are valid, safe, standards-compliant, or appropriate for any specific environment.

The authors and contributors are not responsible for damage, disruption, policy violations, legal issues, data loss, or other consequences resulting from use or misuse of this tool.

## Stop If Unsure

If you are unsure whether you are allowed to send a packet, do not send it. Use the PCAP generation and Wireshark analysis features instead.
