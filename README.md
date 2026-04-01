# Network Port Scanner

A lightweight, multi-threaded TCP port scanner with a graphical user interface built with Python and Tkinter.

## The Need for Network Visibility & Security
In modern network environments, open ports can act as unprotected doors for unauthorized access. This tool provides a fast, reliable way for network administrators, cybersecurity students, and IT auditors to identify exposed TCP ports, verify network configurations, and assess system security.

## Features
- **High-Speed Concurrency** – Utilizes up to 500 concurrent threads to scan thousands of ports rapidly.
- **Service identification** – Automatically resolves well-known ports to their standard services (FTP, SSH, HTTP, HTTPS, MySQL, RDP, etc.).
- **Simple 3-field interface** – Enter a target host, start port, and end port.
- **Real-time feedback** – Live progress bar and elapsed-time tracking during scans.
- **Stop at any time** – Safely cancel a running scan gracefully.
- **Export capabilities** – Save discovered open ports to a `.txt` file for reporting.
- **Cross-platform** – Runs perfectly on Windows, macOS, and Linux.

## Requirements
- Python 3.7 or newer
- Tkinter (Built-in on Windows; on Debian/Ubuntu run `sudo apt-get install python3-tk`)

No third-party packages are required.

## Installation
```bash
git clone https://github.com/basantnema31/Network_scanner.git
cd Network_scanner
```

## Usage
```bash
python portscanergui.py
```
1. Enter the **Target** – An IP address (e.g. `192.168.1.1`) or hostname (e.g. `scanme.nmap.org`).
2. Set the **Start Port** and **End Port** (defaults to `1` – `1024`).
3. Click **Start Scan**. Open ports appear in real time in the results pane.
4. Click **Stop** to cancel a scan early if needed.
5. After a scan completes, click **Save Results** to export the list to a text file.

## Detected Services
This scanner identifies common services dynamically, including but not limited to:
- **21:** FTP
- **22:** SSH
- **80:** HTTP
- **443:** HTTPS
- **3306:** MySQL
- **3389:** RDP

Ports not in the standard map are reported as `Unknown`.

## Disclaimer
Use this tool only on hosts and networks you own or have explicit permission to scan. Unauthorized port scanning may be illegal and violate terms of service policies.

## License
This project is released under the MIT License.
