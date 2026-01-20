Cisco Device Automation using Netmiko
This Python project automates the collection of operational data from Cisco IOS devices using SSH and Telnet with the Netmiko library. Device IP addresses are read from an Excel file, commands are executed automatically, and outputs are saved per device with logging and failure tracking.
🔧 Features
•	SSH and Telnet connectivity using Netmiko
•	Excel-based device input
•	Multiple credential attempts per device
•	Automated execution of Cisco show commands
•	Per-device configuration and status export
•	Timestamped logs for connection and execution status
•	Failed devices highlighted directly in the Excel file
•	Clean, modular code structure suitable for labs and GitHub portfolios
📦 Requirements
•	Python 3.8 or higher
•	Network reachability to Cisco IOS devices
•	Valid Cisco device credentials (SSH and/or Telnet enabled)
🛠 Installation
1. Clone or download this repository.
2. Install required Python libraries:
pip install -r requirements.txt
📄 Input File
An Excel file (.xlsx) containing device IP addresses in the first column. Each row represents one Cisco device.
▶ Usage
SSH Automation:
python cisco_ssh_show_commands.py

Telnet Automation:
python cisco_Telnet_show_commands.py

When prompted, enter the full path to the Excel file.
📁 Output
•	Command output is saved as .txt files (one per device)
•	Logs are written with timestamps for troubleshooting
•	Devices that fail to connect are marked in red inside the Excel file
⚠ Notes
Telnet is intended for lab or legacy environments only. SSH is recommended for production environments.
