Cisco Device Automation using Netmiko

This Python project automates the collection of operational data from Cisco IOS devices using SSH and Telnet with the Netmiko library.
Device IP addresses are read from an Excel file, commands are executed automatically, and outputs are saved per device with logging and failure tracking.

🔧 Features

SSH and Telnet connectivity using Netmiko

Excel-based device input

Multiple credential attempts per device

Automated execution of Cisco show commands

Per-device configuration and status export

Timestamped logs for connection and execution status

Failed devices highlighted directly in the Excel file

Clean, modular code structure suitable for labs and GitHub portfolios

📦 Requirements

Python 3.8 or higher

Network reachability to Cisco IOS devices

Valid Cisco device credentials (SSH and/or Telnet enabled)

🛠 Installation

Clone or download this repository.

Install required Python libraries:

pip install -r requirements.txt

📄 Input File

An Excel file (.xlsx) containing device IP addresses in the first column

Each row represents one Cisco device

Example:

IP Address
192.168.40.8
192.168.40.9
▶ Usage
SSH Automation
python ssh/cisco_ssh_device_collector.py

Telnet Automation
python telnet/cisco_telnet_device_collector.py


When prompted, enter the full path to the Excel file:

C:\path\to\devices.xlsx

📁 Output

Command output is saved as .txt files (one per device)

Logs are written with timestamps for troubleshooting

Devices that fail to connect are marked in red inside the Excel file

⚠ Notes

Telnet is intended for lab or legacy environments only

SSH is recommended for production environments

Executed commands can be customized inside each script
