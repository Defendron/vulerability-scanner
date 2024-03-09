# Vulerability-scanner
I created this vulnerability scanner script as a fun test project. It does the heavy lifting for you:

**Automated scanning of multiple subdomains**: The script asynchronously scans each subdomain for vulnerabilities, making the process efficient and fast.

**Port scanning:** It checks for common vulnerable ports based on historical data, such as FTP, SSH, HTTP, HTTPS, etc.
**Service detection: **After identifying open ports, the script detects the services running on those ports using Nmap's service detection feature.

**Vulnerability scanning**: Based on the detected services, the script performs basic vulnerability checks. Currently, it checks for services associated with Metasploit vulnerabilities.

**Results output:** The scan results, including open ports, detected services, and vulnerability findings, are written to separate files for further analysis.

# How to Use the Vulnerability Scanner Script

This guide will walk you through the steps to use the vulnerability scanner script to scan your subdomains for potential vulnerabilities.

## Prerequisites

Before you begin, ensure that you have the following installed:

- Python 3
- pip (Python package manager)

## Installation

1. Clone the repository to your local machine:
git clone https://github.com/Defendron/vulerability-scanner.git

2. Navigate to the directory containing the script:
cd vulerability-scanner

3. Install the required dependencies:
pip install -r requirements.txt


## Usage

To scan your subdomains for vulnerabilities, follow these steps:

1. Create a file containing a list of subdomains, with one subdomain per line.

2. Run the script, passing the path to the subdomains file as an argument:

python vulnerability_scanner.py subdomains.txt

3. Wait for the script to complete the scanning process. Once finished, the results will be saved to three separate files: `open_ports.txt`, `services.txt`, and `vulnerabilities.txt`.

4. Review the results files to identify any potential vulnerabilities in your subdomains.

## Example

For example, let's say you have a file named `subdomains.txt` containing a list of subdomains:
subdomain1.example.com
subdomain2.example.com
subdomain3.example.com


You would run the script as follows:
python vulnerability_scanner.py subdomains.txt


The script will scan each subdomain for open ports, detect the services running on those ports, and identify any vulnerabilities present.



