# Project Scope: Azure Honeypot with Geolocation Tracking

## Overview
This project involves setting up a honeypot using an Azure Virtual Machine (VM) to gather information on potential attackers. The project leverages Azure Sentinel, custom scripts, and playbooks to visualize attacker data on a map. Below is the detailed scope of the project.

---

## Scope of the Project

### **1. Create a Vulnerable Virtual Machine (VM)**
- Set up a VM in Azure designed to attract attackers by leaving certain services accessible.
- The VM will serve as the honeypot to monitor unauthorized access attempts.

### **2. Gather Log Events and Extract Geolocation**
- Enable logging on the VM to capture events such as login attempts and connection requests.
- Develop a script within the VM to:
  - Parse logs for attacker IP addresses.
  - Use the IP addresses to fetch their longitude and latitude via a geolocation API.

### **3. Integrate with Azure Sentinel**
- Link Azure Sentinel to the resource group containing the VM.
- Use Sentinel to monitor and analyze security-related events.

### **4. Create a Custom Log**
- Create a custom log in the resource group to:
  - Collect data from the script running within the VM.
  - Centralize information on attacker IPs, locations, and timestamps.

### **5. Develop a Playbook for Visualization**
- Create an Azure Sentinel playbook that:
  - Processes the geolocation data from the custom log.
  - Maps the attackers' locations on a geographical visualization.
  - Displays key figures associated with each location (e.g., number of attempts per region).

---

## Goals
1. Understand the origin of attack attempts on the honeypot.
2. Use Azure services to automate the collection and visualization of attacker data.
3. Provide actionable insights using geographical maps for better situational awareness.

---

## Deliverables
1. A working honeypot VM.
2. Script for IP geolocation extraction.
3. Linked Azure Sentinel instance for log monitoring.
4. Custom log for centralized data collection.
5. Visual map showing attack origins with relevant figures.

---

## Assumptions
- The VM will intentionally be left vulnerable for testing and learning purposes.
- The project is conducted in a controlled environment to avoid unintended exposure to malicious actors.

---

## Limitations
- Geolocation accuracy depends on the IP geolocation API used.
- Azure Sentinel’s capabilities may require additional configuration for advanced analysis.
- Familiarity with Azure Playbooks and Sentinel setup is necessary for full implementation.
