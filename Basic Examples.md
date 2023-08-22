1. **Basic Scan** - Discover live hosts within a target network.
   ```bash
   nmap 192.168.1.0/24
   ```

2. **Port Scan** - Specify ports to scan on target hosts.
   ```bash
   nmap -p 80,443 192.168.1.1
   ```

3. **Aggressive Scan** - Comprehensive scan with OS detection, version detection, script scanning, and traceroute.
   ```bash
   nmap -A 192.168.1.1
   ```

4. **Operating System Detection** - Determine the OS running on target hosts.
   ```bash
   nmap -O 192.168.1.1
   ```

5. **Service Version Detection** - Detect versions of services on open ports.
   ```bash
   nmap -sV 192.168.1.1
   ```

6. **UDP Port Scan** - Perform UDP scan on target hosts.
   ```bash
   nmap -sU 192.168.1.1
   ```

7. **Ping Scan (Host Discovery)** - Determine live hosts using ICMP echo requests.
   ```bash
   nmap -sn 192.168.1.0/24
   ```

8. **Script Scan** - Run Nmap scripts against target hosts for more information.
   ```bash
   nmap -sC 192.168.1.1
   ```

9. **Timing Templates** - Adjust scan speed using predefined timing templates.
   ```bash
   nmap -T4 192.168.1.1
   ```

10. **Output Formats** - Specify the output format of scan results.
    ```bash
    nmap -oN scan_results.txt 192.168.1.1
    ```

11. **Exclude Hosts** - Exclude specific hosts from the scan.
    ```bash
    nmap 192.168.1.0/24 --exclude 192.168.1.10
    ```
