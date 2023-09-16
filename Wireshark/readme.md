# Wireshark Usage Guide

Wireshark is an open-source, cross-platform network packet analyzer tool capable of sniffing and investigating live traffic and inspecting PCAP files.

## Overview

Wireshark has the following uses:
- Detecting and troubleshooting network problems, such as network load failure points and congestion.
- Detecting security anomalies, such as rogue hosts, abnormal port usage, and suspicious traffic.
- Investigating and learning protocol details, such as response codes and payload data.

## Interface Overview

Wireshark's interface consists of several components:

- **Toolbar (Red):** The main toolbar contains multiple menus and shortcuts for packet sniffing and processing, including filtering, sorting, summarizing, exporting, and merging.
- **Display Filterbar (Blue):** The main query and filtering section.
- **Capture Filter and Interfaces (Yellow):** Capture filters and available sniffing points. The network interface is the connection point between a computer and a network.
- **Status Bar (Green):** Tool status, profile, and numeric packet information.

![Wireshark Interface](https://github.com/Shawn-Nichol/Tools/assets/30714313/b320f605-183e-4f9f-8860-31ca38c10937)

## Loading PCAP Files

![Loading PCAP Files](https://github.com/Shawn-Nichol/Tools/assets/30714313/217973a0-c210-454f-b6e1-89bbd9764c9d)

Wireshark provides the following views:
- **Packet List:** Summary of each packet (source and destination address, protocol, and packet info).
- **Packet Details Pane:** Detailed protocol breakdown of the selected packet.
- **Packet Bytes Pane:** Hex and decoded ASCII representation of the selected packet. It highlights the packet field depending on the clicked section in the details pane.

## Color Coding

Wireshark uses different colors for packets to highlight conditions and protocols, helping you spot anomalies. You can customize these coloring rules.

## Traffic Sniffing

You can use the shark button to start network sniffing, the red button to stop sniffing, and the green button to restart the sniffing process. The status bar provides information about the sniffing interface and the number of collected packets.

![Traffic Sniffing](https://github.com/Shawn-Nichol/Tools/assets/30714313/4892525c-a73b-457e-b5d0-3a567a795a43)

## Merge Files

Wireshark can combine two pcap files into one single file using the "File --> Merge" option.

## Viewing Packet Details

Wireshark allows you to view packet details, including layers based on the OSI model.

- **Layer 1 (Frame):** Details specific to the physical layer of the OSI model.
![Layer 1](https://github.com/Shawn-Nichol/Tools/assets/30714313/8b01405d-7471-4b24-8411-310badf2e106)

- **Layer 2 (Source, MAC):** Source and destination MAC addresses from the Data Link layer.
![Layer 2](https://github.com/Shawn-Nichol/Tools/assets/30714313/e6fd9930-3e20-44d0-bbf1-55419055aa4c)

- **Layer 3 (Source, IP):** Source and destination IP addresses from the network layer.
![Layer 3](https://github.com/Shawn-Nichol/Tools/assets/30714313/f7f84d9c-b113-409e-ab85-ad1f70d3a1e3)

- **Layer 4 (Protocol):** Details of the protocol used (UDP/TCP) and source and destination ports from the Transport Layer.
![Layer 4](https://github.com/Shawn-Nichol/Tools/assets/30714313/1c73af8c-2416-45c9-b6af-e72112a1c770)

- **Layer 5 (Application Protocol):** Details specific to the protocol used, such as HTTP, FTP, and SMB, from the Application layer.
![Layer 5](https://github.com/Shawn-Nichol/Tools/assets/30714313/acadbb71-638d-49f7-87b1-45a628b32cb9)

## Packet Navigation

Wireshark assigns a unique number to each packet, making finding and investigating specific packets easier, especially in large captures.

## Finding Packets

Wireshark can find packets by content. Use the "Edit --> Find Packet" menu to search for specific events of interest. You can search by display filters, hex values, strings, or regex patterns.

## Marking Packets

Mark packets to point to specific events of interest for further investigation. Marked packets are shown in black, regardless of the original color.

## Packet Comments

Add comments to packets to aid in further investigation or to highlight important/suspicious points for analysis.

## Severity Chart

Wireshark uses different colors to indicate severity levels:
- Blue: Information on usual workflow.
- Cyan: Notable events like application error codes.
- Yellow: Warnings like unusual error codes or problem statements.
- Red: Problems like malformed packets.

## Packet Filtering

There are two types of filtering in Wireshark:
- Capture Filters: Capture only packets valid for the specified filter.
- Display Filters: Used for viewing packets that match the specified filter.

You can also right-click on an event instead of writing a rule to filter for that type of event.

## Conversation Filter

Use conversation filters to analyze specific values in packets.

## Colorize Conversation

Change color rules for conversations without regard for previous rules.

## Follow Stream

Reconstruct the stream and view raw traffic as presented at the application level. This helps analysts recreate application-level data and understand events of interest. Use "Analyze --> Follow TCP/UDP/HTTP Stream" for this purpose.
