### ipconfig Command


<table>
  <caption><code>ipconfig</code> Command</caption>
  <tr>
    <th>Tag</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td><code>/all</code></td>
    <td>Displays detailed IP configuration for all network interfaces.</td>
    <td><code>ipconfig /all</code></td>
  </tr>
  <tr>
    <td><code>/release</code></td>
    <td>Releases the DHCP-assigned IP address for a network interface.</td>
    <td><code>ipconfig /release</code></td>
  </tr>
  <tr>
    <td><code>/renew</code></td>
    <td>Renews the DHCP-assigned IP address for a network interface.</td>
    <td><code>ipconfig /renew</code></td>
  </tr>
</table>


### ping Command


<table>
  <caption><code>ping</code> Command</caption>
  <tr>
    <th>Tag</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td><code>-t</code></td>
    <td>Continuously pings the target until manually stopped.</td>
    <td><code>ping -t google.com</code></td>
  </tr>
  <tr>
    <td><code>-n</code></td>
    <td>Specifies the number of echo requests to send.</td>
    <td><code>ping -n 5 google.com</code></td>
  </tr>
</table>


### tracert Command


<table>
  <caption><code>tracert</code> Command</caption>
  <tr>
    <th>Tag</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td><code>-d</code></td>
    <td>Prevents the resolution of IP addresses to hostnames.</td>
    <td><code>tracert -d google.com</code></td>
  </tr>
  <tr>
    <td><code>-h</code></td>
    <td>Specifies the maximum number of hops to trace.</td>
    <td><code>tracert -h 10 google.com</code></td>
  </tr>
</table>


### netstat

<table>
  <caption><code>netstat</code> Commands</caption>
  <tr>
    <th>Tag</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>No specific tags</td>
    <td>Displays network statistics and active connections.</td>
    <td><code>netstat</code></td>
  </tr>
  <tr>
    <td><code>-a</code></td>
    <td>Displays all listening and non-listening ports.</td>
    <td><code>netstat -a</code></td>
  </tr>
  <tr>
    <td><code>-n</code></td>
    <td>Displays addresses and port numbers in numerical form.</td>
    <td><code>netstat -n</code></td>
  </tr>
  <tr>
    <td><code>-o</code></td>
    <td>Displays the owning process ID associated with each connection.</td>
    <td><code>netstat -o</code></td>
  </tr>
  <tr>
    <td><code>-p [protocol]</code></td>
    <td>Displays connections for a specific protocol (e.g., TCP or UDP).</td>
    <td><code>netstat -p tcp</code></td>
  </tr>
  <tr>
    <td><code>-s</code></td>
    <td>Displays per-protocol statistics.</td>
    <td><code>netstat -s</code></td>
  </tr>
  <tr>
    <td><code>-r</code></td>
    <td>Displays the routing table.</td>
    <td><code>netstat -r</code></td>
  </tr>
  <tr>
    <td><code>-b</code></td>
    <td>Displays the executable involved in creating each connection or listening port.</td>
    <td><code>netstat -b</code></td>
  </tr>
</table>

### nslookup

<table>
  <caption><code>nslookup</code> Commands</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>No specific tags</td>
    <td><code>nslookup google.com</code></td>
    <td>Queries DNS servers to resolve hostnames to IP addresses.</td>
  </tr>
  <tr>
    <td><code>-type=[record type]</code></td>
    <td><code>nslookup -type=MX google.com</code></td>
    <td>Specifies the type of DNS record to query (e.g., MX, A, CNAME).</td>
  </tr>
  <tr>
    <td><code>-server=[DNS server]</code></td>
    <td><code>nslookup -server=8.8.8.8 google.com</code></td>
    <td>Specifies the DNS server to use for the query.</td>
  </tr>
</table>

### arp

<table>
  <caption><code>arp</code> Commands</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>-a</code></td>
    <td><code>arp -a</code></td>
    <td>Displays the ARP cache, which maps IP addresses to MAC addresses.</td>
  </tr>
  <tr>
    <td><code>-d [IP address]</code></td>
    <td><code>arp -d 192.168.1.1</code></td>
    <td>Deletes an entry from the ARP cache for a specific IP address.</td>
  </tr>
  <tr>
    <td><code>-s [IP address] [MAC address]</code></td>
    <td><code>arp -s 192.168.1.1 00-1A-2B-3C-4D-5E</code></td>
    <td>Adds a static ARP entry, mapping an IP address to a MAC address.</td>
  </tr>
  <tr>
    <td><code>-d *</code></td>
    <td><code>arp -d *</code></td>
    <td>Clears all entries from the ARP cache.</td>
  </tr>
</table>

### nbstat

<table>
  <caption><code>nbtstat</code> Commands</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>-a [IP address]</code></td>
    <td><code>nbtstat -a 192.168.1.1</code></td>
    <td>Displays NetBIOS over TCP/IP statistics for a specific IP address.</td>
  </tr>
  <tr>
    <td><code>-A [hostname]</code></td>
    <td><code>nbtstat -A computername</code></td>
    <td>Displays NetBIOS over TCP/IP statistics for a specific hostname.</td>
  </tr>
  <tr>
    <td><code>-c</code></td>
    <td><code>nbtstat -c</code></td>
    <td>Lists the NetBIOS name cache, which maps NetBIOS names to IP addresses.</td>
  </tr>
  <tr>
    <td><code>-n</code></td>
    <td><code>nbtstat -n</code></td>
    <td>Lists local NetBIOS name tables, which include registered NetBIOS names.</td>
  </tr>
  <tr>
    <td><code>-R</code></td>
    <td><code>nbtstat -R</code></td>
    <td>Purges and reloads the remote cache name table.</td>
  </tr>
</table>


### route

<table>
  <caption><code>route</code> Commands</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>No specific tags</td>
    <td><code>route print</code></td>
    <td>Displays the IP routing table, which contains routing information for network traffic.</td>
  </tr>
  <tr>
    <td><code>add [destination] [mask] [gateway] [metric]</code></td>
    <td><code>route add 192.168.2.0 mask 255.255.255.0 192.168.1.1 metric 10</code></td>
    <td>Adds a route to the routing table for a specific destination network.</td>
  </tr>
  <tr>
    <td><code>delete [destination]</code></td>
    <td><code>route delete 192.168.2.0</code></td>
    <td>Deletes a route from the routing table for a specific destination network.</td>
  </tr>
  <tr>
    <td><code>change [destination] [mask] [gateway] [metric]</code></td>
    <td><code>route change 192.168.2.0 mask 255.255.255.0 192.168.1.2 metric 20</code></td>
    <td>Modifies an existing route in the routing table for a specific destination network.</td>
  </tr>
  <tr>
    <td><code>-p</code></td>
    <td><code>route -p add 192.168.2.0 mask 255.255.255.0 192.168.1.1 metric 10</code></td>
    <td>Makes a route persistent (survives reboots) by using the -p option with the add command.</td>
  </tr>
</table>


### netsh

<table>
  <caption><code>netsh</code> Commands</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>No specific tags</td>
    <td><code>netsh</code></td>
    <td>Opens the `netsh` command prompt, allowing you to configure various network settings and services.</td>
  </tr>
  <tr>
    <td><code>interface show interface</code></td>
    <td><code>netsh interface show interface</code></td>
    <td>Displays a list of all network interfaces on the system.</td>
  </tr>
  <tr>
    <td><code>interface ipv4 show addresses</code></td>
    <td><code>netsh interface ipv4 show addresses</code></td>
    <td>Displays the IPv4 addresses assigned to network interfaces.</td>
  </tr>
  <tr>
    <td><code>firewall show currentprofile</code></td>
    <td><code>netsh firewall show currentprofile</code></td>
    <td>Shows the current Windows Firewall profile settings.</td>
  </tr>
  <tr>
    <td><code>wlan show profiles</code></td>
    <td><code>netsh wlan show profiles</code></td>
    <td>Lists wireless network profiles saved on the computer.</td>
  </tr>
  <tr>
    <td><code>advfirewall show allprofiles</code></td>
    <td><code>netsh advfirewall show allprofiles</code></td>
    <td>Displays information about the advanced firewall settings for all profiles (domain, private, and public).</td>
  </tr>
  <tr>
    <td><code>dhcp show server</code></td>
    <td><code>netsh dhcp show server</code></td>
    <td>Shows the list of DHCP servers on the network.</td>
  </tr>
</table>


### Hostname


<table>
  <caption><code>hostname</code> Command</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>No specific tags</td>
    <td><code>hostname</code></td>
    <td>Displays the computer's hostname, which is the unique name assigned to the computer on a network.</td>
  </tr>
  <tr>
    <td><code>-I [interface]</code></td>
    <td><code>hostname -I eth0</code></td>
    <td>Displays the IP address associated with a specific network interface.</td>
  </tr>
  <tr>
    <td><code>-d [domain]</code></td>
    <td><code>hostname -d example.com</code></td>
    <td>Sets the computer's DNS domain name (part of the Fully Qualified Domain Name or FQDN).</td>
  </tr>
  <tr>
    <td><code>-b [name]</code></td>
    <td><code>hostname -b mycomputer</code></td>
    <td>Sets the computer's hostname to a specific name.</td>
  </tr>
</table>


### telnet

<table>
  <caption><code>telnet</code> Command</caption>
  <tr>
    <th>Tag</th>
    <th>Example</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>No specific tags</td>
    <td><code>telnet example.com</code></td>
    <td>Establishes a Telnet connection to a remote host using the default port (23).</td>
  </tr>
  <tr>
    <td><code>[hostname] [port]</code></td>
    <td><code>telnet example.com 80</code></td>
    <td>Connects to a specific port on a remote host.</td>
  </tr>
  <tr>
    <td><code>-a [remote host]</code></td>
    <td><code>telnet -a example.com</code></td>
    <td>Logs in automatically with the current user's credentials when connecting to a remote host.</td>
  </tr>
  <tr>
    <td><code>-l [username]</code></td>
    <td><code>telnet -l myuser example.com</code></td>
    <td>Logs in with a specified username when connecting to a remote host.</td>
  </tr>
  <tr>
    <td><code>-e [escape character]</code></td>
    <td><code>telnet -e ^] example.com</code></td>
    <td>Specifies an escape character to control Telnet commands.</td>
  </tr>
</table>



