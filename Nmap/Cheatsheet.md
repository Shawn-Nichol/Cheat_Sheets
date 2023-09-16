## Port Specific 

<table>
  <tr>
    <th style="background-color: orange;">Option</th>
    <th style="background-color: orange;">Description</th>
    <th style="background-color: orange;">Syntax and Example</th>
  </tr>
  <tr>
    <td>-p</td>
    <td>Scan specific port</td>
    <td><code>nmap -p 53 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-p</td>
    <td>Scan specific port range</td>
    <td><code>nmap -p 20-100 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-pU</td>
    <td>Scan UDP</td>
    <td><code>nmap -pU:100 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-p-</td>
    <td>Scan all ports</td>
    <td><code>nmap -p- 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-p</td>
    <td>Scan specified protocols</td>
    <td><code>nmap -p smtp,dns 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-F</td>
    <td>Fast port scan</td>
    <td><code>nmap -F 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-r</td>
    <td>Sequential port scan</td>
    <td><code>nmap -r 192.168.1.1</code></td>
  </tr>
</table>

## Host Discovery Options


<table>
  <tr>
    <th style="background-color: orange;">Option</th>
    <th style="background-color: orange;">Description</th>
    <th style="background-color: orange;">Syntax and Example</th>
  </tr>
  <tr>
    <td>-sn</td>
    <td>Ping scan (disable port scan)</td>
    <td><code>nmap -sn 192.168.1.0/24</code></td>
  </tr>
  <tr>
    <td>-Pn</td>
    <td>No ping (skip host discovery)</td>
    <td><code>nmap -Pn 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-PE</td>
    <td>Enable ICMP echo (ping) discovery</td>
    <td><code>nmap -PE 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-PS</td>
    <td>Enable TCP SYN ping discovery</td>
    <td><code>nmap -PS 80 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-PU</td>
    <td>Enable UDP ping discovery</td>
    <td><code>nmap -PU 161 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-n</td>
    <td>No DNS resolution</td>
    <td><code>nmap -n 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-PA</td>
    <td>Enable ARP ping discovery</td>
    <td><code>nmap -PA 192.168.1.1</code></td>
  </tr>
</table>

## Scanning Types

<table>
  <tr>
    <th style="background-color: orange;">Option</th>
    <th style="background-color: orange;">Description</th>
    <th style="background-color: orange;">Syntax and Example</th>
  </tr>
  <tr>
    <td>-sA</td>
    <td>ACK scan (TCP ACK scan)</td>
    <td><code>nmap -sA 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-sS</td>
    <td>Stealth SYN scan (TCP SYN scan)</td>
    <td><code>nmap -sS 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-sT</td>
    <td>Connect scan (TCP connect scan)</td>
    <td><code>nmap -sT 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-sU</td>
    <td>UDP scan</td>
    <td><code>nmap -sU 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-sX</td>
    <td>XMAS scan</td>
    <td><code>nmap -sX 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-SF</td>
    <td>FTP bounce scan</td>
    <td><code>nmap -SF 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-SL</td>
    <td>Idle scan</td>
    <td><code>nmap -SL 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-Sp</td>
    <td>Ping scan (no port scan)</td>
    <td><code>nmap -Sp 192.168.1.0/24</code></td>
  </tr>
</table>

## Version Scanning

<table>
  <tr>
    <th style="background-color: orange;">Option</th>
    <th style="background-color: orange;">Description</th>
    <th style="background-color: orange;">Syntax and Example</th>
  </tr>
  <tr>
    <td>-sV</td>
    <td>Service version detection</td>
    <td><code>nmap -sV 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>--version-intensity</td>
    <td>Set version detection intensity (0-9)</td>
    <td><code>nmap --version-intensity 5 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>--version-all</td>
    <td>Attempt to identify all versions</td>
    <td><code>nmap --version-all 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>--version-light</td>
    <td>Lighter banner grabbing detection</td>
    <td><code>nmap --version-light 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>--version-trace</td>
    <td>Show detailed version scan activity</td>
    <td><code>nmap --version-trace 192.168.1.1</code></td>
  </tr>
</table>


## Timing Options

<table>
  <tr>
    <th style="background-color: orange;">Option</th>
    <th style="background-color: orange;">Description</th>
    <th style="background-color: orange;">Syntax and Example</th>
  </tr>
  <tr>
    <td>-T0</td>
    <td>Paranoid timing (slowest)</td>
    <td><code>nmap -T0 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-T1</td>
    <td>Sneaky timing (very slow)</td>
    <td><code>nmap -T1 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-T2</td>
    <td>Polite timing (slow)</td>
    <td><code>nmap -T2 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-T3</td>
    <td>Normal timing (default)</td>
    <td><code>nmap -T3 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-T4</td>
    <td>Aggressive timing (fast)</td>
    <td><code>nmap -T4 192.168.1.1</code></td>
  </tr>
  <tr>
    <td>-T5</td>
    <td>Insane timing (fastest)</td>
    <td><code>nmap -T5 192.168.1.1</code></td>
  </tr>
</table>
