# Cisco Device Automation using Netmiko

## Overview
This repository provides Python automation scripts to collect operational data from Cisco IOS devices using Netmiko.
It supports both SSH and Telnet connections and uses an Excel file as input for device IP addresses.

The scripts are designed for lab, testing, and learning purposes and follow a clean, modular structure suitable for GitHub portfolios.

---

## Features
- SSH and Telnet support
- Excel-based device input
- Multiple credential attempts
- Automated execution of Cisco show commands
- Per-device output files
- Logging for troubleshooting
- Failed devices highlighted directly in Excel

---

## Repository Structure
cisco-device-automation-netmiko/
│
├── ssh/
│ └── cisco_ssh_device_collector.py
│
├── telnet/
│ └── cisco_telnet_device_collector.py
│
├── input/
│ └── IPS.xlsx
│
├── output/
│ └── .gitkeep
│
├── logs/
│ └── .gitkeep
│
├── requirements.txt
├── README.md
└── .gitignore

---

##Requirements
• Python 3.8 or higher
• Netmiko
• openpyxl

---

##Input File Format
The Excel file must contain device IP addresses in the first column only. Each row represents a single device.

---

##Usage
SSH Automation:
python ssh/cisco_ssh_device_collector.py

Telnet Automation:
python telnet/cisco_telnet_device_collector.py

When prompted, provide the full path to the Excel file.

---

##Output
• Command outputs are saved as text files per device
• Logs are stored in the logs directory
• Failed devices are marked in red inside the Excel file

---

##Notes
Telnet is intended for lab or legacy environments only. SSH is recommended for production environments.

