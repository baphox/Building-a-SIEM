## Building a SIEM

# Objective

The primary objective of building a Security Information and Event Management (SIEM) system is to enhance an organization's ability to detect, respond to, and mitigate cybersecurity threats effectively. 

# Diagram

<img src="https://i.imgur.com/VtnkAJu.png" alt="Wazuh Automation Diagram 1">

# System Requirements

|     Agents     |                 CPU                |     RAM       |      Storage (90days)       |
| --------------- | ------------------------------------- | --------------- | --------------- |
|       1-25          |                4 vCPU                       |     8 GiB           |       50 GB          |
|       25-50          |                8 vCPU                       |     8 GiB           |       100 GB          |
|       50-100          |                8 vCPU                       |     8 GiB           |       200 GB          |

# Creating a new server for installation

<img src="https://i.imgur.com/6XrGaMb.png" alt="Creating a droplet for Wazuh Step 1">
<img src="https://i.imgur.com/1N4aPUk.png" alt="Creating a droplet for Wazuh Step 2">
<img src="https://i.imgur.com/uY8vFkM.png" alt="Creating a droplet for Wazuh Step 3">
<img src="https://i.imgur.com/Guf0VP2.png" alt="Creating a droplet for Wazuh Step 4">
<img src="https://i.imgur.com/Xbq43XO.png" alt="Creating a droplet for Wazuh Step 5">

# Creating Firewall

<img src="https://i.imgur.com/peOlIw1.png" alt="Creating a Firewall Step 1">
<img src="https://i.imgur.com/l2lptyM.png" alt="Creating a Firewall Step 2">
<img src="https://i.imgur.com/gH9vmMf.png" alt="Creating a Firewall Step 3">
<img src="https://i.imgur.com/2rUs3Vh.png" alt="Creating a Firewall Step 4">

# Install Wazuh

Install Wazuh 4.7
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh && sudo bash ./wazuh-install.sh -a

Extract Wazuh Credentials
sudo tar -xvf wazuh-install-files.tar

# Monitoring and Logging

Set up monitoring and logging tools to track the performance and health of your home lab environment. Tools like Prometheus, Grafana, and ELK stack provide insights into system behavior and performance.

# Security Measures

Implement security measures to protect your home lab environment. Configure firewalls, set up VPNs, use strong passwords, and keep software updated to safeguard against unauthorized access and threats.

# Backup and Recovery

Implement backup and recovery solutions to prevent data loss. Regularly backup your data and test the restoration process to ensure it functions as expected in case of hardware failure or system crashes.
