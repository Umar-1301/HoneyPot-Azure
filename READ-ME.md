# Azure Honeypot with Geolocation Tracking

## Overview
This project demonstrates the creation of a honeypot using Azure Virtual Machines (VMs) to track and analyze attack attempts. The honeypot collects data about attackers, extracts geolocation information, and visualizes their origins on a map using Azure Sentinel and PowerShell scripts.

---

## Features
- **Vulnerable VM Setup**: A deliberately vulnerable Azure VM to attract attackers.
- **Geolocation Tracking**: PowerShell script to extract longitude and latitude of attackers based on IP addresses.
- **Azure Sentinel Integration**: Automated monitoring and analysis of attack logs.
- **Custom Log Management**: Centralized logging of attack data in Azure resource groups.
- **Map Visualization**: A playbook to visualize attacker locations and figures on a map.

---

## Prerequisites
To replicate this project, ensure you have:
1. An active Azure account with the necessary permissions.
2. Basic knowledge of Azure Virtual Machines and Azure Sentinel.
3. Familiarity with PowerShell scripting.

---

## Project Structure
- `SCOPE.md`: Defines the scope and objectives of the project.
- `scripts/`:
  - `geolocation_script.ps1`: Extracts geolocation data from attacker IPs.
  - `map_visualization_playbook.json`: The Azure Sentinel playbook for mapping.
- `example_logs.txt`: Sample logs showing attacker data.
- `INSTALL.md`: Step-by-step installation and setup guide.
- `LICENSE`: License information for this project.

---

## How It Works
1. **Vulnerable VM Creation**:
   - Set up a virtual machine with intentional vulnerabilities to attract unauthorized access attempts.
2. **Log Collection**:
   - Enable logging to capture events such as login attempts.
   - Use a PowerShell script to parse logs and extract attacker IPs.
3. **Geolocation Extraction**:
   - The PowerShell script fetches longitude and latitude data for each attacker IP using a geolocation API.
4. **Azure Sentinel Integration**:
   - Link Sentinel to the resource group containing the VM.
   - Create a custom log to collect geolocation data.
5. **Map Visualization**:
   - Use an Azure Sentinel playbook to display attacker locations on a map with relevant statistics.

---

## Getting Started
1. **Set Up the VM**:
   - Follow the instructions in `INSTALL.md` to deploy and configure the honeypot VM.
2. **Run the Script**:
   - Deploy the `geolocation_script.ps1` within the VM.
   - Configure the script to gather log data and fetch geolocation information.
3. **Integrate Azure Sentinel**:
   - Link Sentinel to your resource group.
   - Import the `map_visualization_playbook.json` into Sentinel.
4. **Visualize Data**:
   - Run the playbook to visualize the attacker data on a map.

---
