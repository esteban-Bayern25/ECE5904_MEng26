# ZigBee vs. Mist IoT Protocol Security Analysis
**ECE 5904 — MEng Capstone Report | Virginia Tech, 2026**  
Esteban Rodriguez · Bradley Department of Electrical and Computer Engineering

## About this repository

This repository contains the supplementary datasets and raw packet captures 
referenced in Appendix B of the report:

> *ZigBee vs. Mist IoT Protocol Analysis* — a comparative security audit 
> evaluating interception depth across ZigBee 3.0 and Mist (LwMesh) 
> architectures using a unified nRF52840-based hardware sniffer.

## Repository structure
[Pcap Files](/pcap_captures)


## How to use the PCAP files

1. Install [Wireshark](https://www.wireshark.org/)
2. Open any `.pcap` file
3. To decrypt ZigBee traffic, load the Network Key via:  
   **Edit → Preferences → Protocols → ZigBee → Add key**
4. Filter for the Transport Key exchange using:  
   `zbee_nwk.cmd.id == 0x05`
