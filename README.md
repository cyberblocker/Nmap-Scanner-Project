**About**

This project is a Python-based network reconnaissance tool designed to run on a Kali Linux VM. It supports both defensive (blue team) and offensive (red team) use cases by automating common network enumeration tasks.

**What It Does**

The tool enumerates a /20 subnet based on a user-provided IP address. It uses a menu-driven interface with three core functions:

  - Ping Scan – Identifies active hosts within the subnet
  - Port Scan – Scans discovered hosts for open ports within a specified range
  - Version Scan – Detects service versions running on open ports
  
**Requirements**
  - Python
  - Kali Linux (recommended environment)
  - Nmap installed and configured

**Usage**
**Input Format**
  - Enter a valid IPv4 address (e.g., 192.168.1.1)
  - Invalid formats will be rejected by the program
**1. Ping Scan**
  - Performs host discovery across a /20 subnet using Nmap
  - Identifies active IP addresses without scanning ports
  - May take some time depending on network size
**2. Port Scan**
  - Scans open ports on discovered IP addresses
  - Requires a user-defined port range (start port must be lower than end port)
  - Helps identify exposed services and potential attack surfaces
**3. Version Scan**
  - Uses nmap -sV to detect service versions on open ports
  - Iterates through discovered IPs and scans each host
  - Provides detailed service information (name, version, etc.)
  - Useful for vulnerability assessment and security analysis
  - Scan duration may vary depending on network size

**How It Works**

The program automates Nmap commands through Python, streamlining the process of:

1. Discovering hosts
2. Identifying open ports
3. Analyzing running services

This reduces manual effort and speeds up network reconnaissance workflows.

**Use Cases**
  - Network auditing
  - Vulnerability assessment
  - Security testing (red/blue team exercises)
  - Learning and lab environments

**Conclusion**

This tool simplifies network enumeration by combining host discovery, port scanning, and service analysis into a single workflow. It is designed to save time and improve efficiency when analyzing network environments.
networks security professionals can use this automation to save time by helping to simplify redundant tasks.
