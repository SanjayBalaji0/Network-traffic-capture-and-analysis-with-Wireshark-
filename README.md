# Network-traffic-capture-and-analysis-with-Wireshark

### Name : Sanjay Balaji S
### Reg. No : 212223240149

## AIM:
To capture and analyze network traffic using Wireshark in order to observe protocols, packets, and potential anomalies.
## Requirements:
- **Hardware:**
    - Computer with internet access
    - Network adapter (Ethernet/Wi-Fi)
- **Software:**
    - Wireshark (latest stable version)
    - Sample PCAP files (optional for offline analysis)
## Architecture:
```mermaid
flowchart TD
    A[Network Interface Card] --> B[Wireshark Packet Capture Engine]
    B --> C[Packet Decoder & Protocol Analyzer]
    C --> D[Packet Display & Filtering Interface]
    D --> E[Investigator Analyzes Network Data]
    E --> F[Findings: IPs, Ports, Protocols, Anomalies]
```
## DESIGN STEPS:
### Step 1:
Install Wireshark on the system.

### Step 2:
Launch Wireshark and select the network interface (Ethernet/Wi-Fi).

### Step 3:
Start the capture, apply filters (like http, tcp, ip.addr == x.x.x.x) to analyze specific traffic, and stop the capture after observing relevant data.
### Step 4:
**Analyze traffic to identify:**
  - Source & Destination IP addresses
  - Protocols (HTTP, DNS, TCP, UDP, etc.)
  - Suspicious activities (e.g., unusual ports, repeated requests).
## PROGRAM:
Wireshark Packet Capture and Filter Usage

![alt text](<Screenshot 2025-10-08 080930.png>)


Start Capturing Packets

• Click the blue shark fin icon or double-click the interface.

• Wireshark will start capturing all real-time traffic.

![alt text](<Screenshot 2025-10-08 080954.png>)

![alt text](<Screenshot 2025-10-08 081016.png>)

Apply Filters to Focus on Specific Traffic

• Use filters like http, ip.addr == 192.168.1.1, or tcp.port == 80 in the top filter bar to narrow down results.

![alt text](<Screenshot 2025-10-08 081114.png>)


Analyze Packet Details

• Click on a packet to view its detailed breakdown including frame, Ethernet,IP, TCP/UDP layers, and data payload.

Captured Packets with Protocol Analysis and Detailed Packet Info

![alt text](<Screenshot 2025-10-08 081126.png>)


## RESULT:
Network traffic was successfully captured and analyzed using Wireshark.
