# Network Traffic Analyzer 

## Overview
This is a high-performance Python tool designed to analyze network traffic characteristics across different applications (Web, Video, Audio, etc.). It performs Deep Packet Inspection (DPI) on PCAP files to extract and visualize protocol distributions, IP header fields, and TCP/UDP parameters.

## Technical Features
- **Strict TLS Detection:** Implements logic similar to Wireshark for accurate TLS record detection.
- **QUIC Protocol Support:** Specialized detection for QUIC connections over UDP.
- **Comprehensive Analytics:** Extracts metrics for:
    - IP Header fields (TTL, IHL, ToS, Flags).
    - TCP Window sizes and Option headers.
    - Packet size distribution and traffic directionality.
- **Advanced Visualizations:** Automatically generates CDF plots for inter-arrival times and categorical packet size distributions.

## Design & Architecture
The tool is built using **Object-Oriented Programming (OOP)** for modularity and scalability:
- **`TrafficAnalyzer` Class:** Centralizes the analysis logic, feature extraction, and reporting.
- **Data Persistence:** Uses **Pandas DataFrames** for efficient manipulation of network metadata.


## Getting Started
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
