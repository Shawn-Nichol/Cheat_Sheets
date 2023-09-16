## Interface Overview

Wireshark's interface consists of several components:

- **Toolbar (Red):** The main toolbar contains multiple menus and shortcuts for packet sniffing and processing, including filtering, sorting, summarizing, exporting, and merging.
- **Display Filterbar (Blue):** The main query and filtering section.
- **Capture Filter and Interfaces (Yellow):** Capture filters and available sniffing points. The network interface is the connection point between a computer and a network.
- **Status Bar (Green):** Tool status, profile, and numeric packet information.

![Wireshark Interface](https://github.com/Shawn-Nichol/Tools/assets/30714313/b320f605-183e-4f9f-8860-31ca38c10937)

## Loading PCAP Files

![Loading PCAP Files](https://github.com/Shawn-Nichol/Tools/assets/30714313/217973a0-c210-454f-b6e1-89bbd9764c9d)

Wireshark provides multiple views for analyzing network packets:

- **Packet List:** A summary of each packet, including source and destination addresses, protocol, and packet information.
- **Packet Details Pane:** Offers a detailed breakdown of the selected packet's protocol layers.
- **Packet Bytes Pane:** Displays the packet's hexadecimal and decoded ASCII representations, highlighting fields when selected in the details pane.

## Color Coding

Wireshark employs various packet colors to highlight conditions and protocols, assisting in identifying anomalies. You can customize these coloring rules.

## Traffic Sniffing

Wireshark provides convenient controls for network sniffing:

- The "shark" button initiates network sniffing.
- The red button stops the sniffing process.
- The green button restarts the sniffing.

The status bar displays information about the sniffing interface and the number of collected packets.

![Traffic Sniffing](https://github.com/Shawn-Nichol/Tools/assets/30714313/4892525c-a73b-457e-b5d0-3a567a795a43)

## Merging Files

Wireshark allows you to merge two pcap files into a single file using the "File --> Merge" option.

## Viewing Packet Details

Wireshark facilitates in-depth analysis of packet details, organized according to the OSI model layers:

- **Layer 1 (Frame):** Specifics pertaining to the physical layer of the OSI model.
![Layer 1](https://github.com/Shawn-Nichol/Tools/assets/30714313/8b01405d-7471-4b24-8411-310badf2e106)

- **Layer 2 (Source, MAC):** Source and destination MAC addresses from the Data Link layer.
![Layer 2](https://github.com/Shawn-Nichol/Tools/assets/30714313/e6fd9930-3e20-44d0-bbf1-55419055aa4c)

- **Layer 3 (Source, IP):** Source and destination IP addresses from the network layer.
![Layer 3](https://github.com/Shawn-Nichol/Tools/assets/30714313/f7f84d9c-b113-409e-ab85-ad1f70d3a1e3)

- **Layer 4 (Protocol):** Details of the protocol used (UDP/TCP) and source and destination ports from the Transport Layer.
![Layer 4](https://github.com/Shawn-Nichol/Tools/assets/30714313/1c73af8c-2416-45c9-b6af-e72112a1c770)

- **Layer 5 (Application Protocol):** Protocol-specific details, such as HTTP, FTP, and SMB, from the Application layer.
![Layer 5](https://github.com/Shawn-Nichol/Tools/assets/30714313/acadbb71-638d-49f7-87b1-45a628b32cb9)

## Packet Navigation

Wireshark assigns a unique number to each packet, simplifying finding and investigating specific packets, especially in large captures.
