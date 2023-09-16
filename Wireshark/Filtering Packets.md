## Finding Packets

Wireshark offers several methods to find packets of interest:

- **Edit --> Find Packet:** Use this menu option to search for specific events, packets, or data patterns. You can search by display filters, hex values, strings, or regular expressions.

## Marking Packets

Marking packets can be a valuable technique for highlighting specific events during analysis. Marked packets are displayed in black, making them easily distinguishable from other packets.

## Packet Comments

Adding comments to packets can enhance your investigative process. Use comments to annotate important or suspicious points, helping you keep track of notable findings during your analysis.

## Severity Chart

Wireshark employs a color-coded severity chart to help you quickly identify the significance of events:

- **Blue:** Represents information about regular workflow or expected behavior.
- **Cyan:** Indicates notable events, such as application error codes or significant protocol events.
- **Yellow:** Highlights warnings, such as unusual error codes or potential problem statements.
- **Red:** Signals critical problems, such as malformed packets or severe network issues.

## Packet Filtering

Wireshark provides two types of filtering mechanisms:

- **Capture Filters:** Use capture filters to capture only the packets that meet specific criteria. This is useful for capturing relevant data from a high-volume network traffic stream.
- **Display Filters:** Display filters allow you to view packets that match specific criteria while analyzing captured data. You can also right-click on an event and apply a quick filter to see packets related to that event.

## Conversation Filter

Conversation filters enable you to focus on specific values or interactions within packets. This is particularly helpful when you want to analyze communication between specific endpoints or with specific attributes.

## Colorize Conversation

Wireshark allows you to customize color rules for conversations, providing flexibility in how you visualize and distinguish different types of network traffic.

## Follow Stream

To better understand application-level data and analyze events of interest, you can use the "Analyze --> Follow TCP/UDP/HTTP Stream" feature. This function reconstructs the stream and presents raw traffic at the application level, aiding analysts in recreating and comprehending application-level data flow.
