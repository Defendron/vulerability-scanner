# vulerability-scanner
I created this vulnerability scanner script as a fun test project. It does the heavy lifting for you:

**Automated scanning of multiple subdomains**: The script asynchronously scans each subdomain for vulnerabilities, making the process efficient and fast.

**Port scanning:** It checks for common vulnerable ports based on historical data, such as FTP, SSH, HTTP, HTTPS, etc.
**Service detection: **After identifying open ports, the script detects the services running on those ports using Nmap's service detection feature.

**Vulnerability scanning**: Based on the detected services, the script performs basic vulnerability checks. Currently, it checks for services associated with Metasploit vulnerabilities.

**Results output:** The scan results, including open ports, detected services, and vulnerability findings, are written to separate files for further analysis.
