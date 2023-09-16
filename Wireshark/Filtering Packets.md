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
