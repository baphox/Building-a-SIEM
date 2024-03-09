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
```
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
```
Extract Wazuh Credentials
```
sudo tar -xvf wazuh-install-files.tar
```

Now we need the Wazuh Credentials
```
ls
```
```
cd wazuh-install-files/
```
```
ls
```
```
cat wazuh-passwords.txt
```
<img src="https://i.imgur.com/H9OdKD7.png" alt="Wazuh Credentials">

# Deploy Agent on Wazuh using Windows

Once we login to our Wazuh Dashboard using our Credentials we can see on the left corner the Add Agent button
<img src="https://i.imgur.com/Pl5YuFz.png" alt="Wazuh Deploy Agent Step 1">

Let's click that!

Server address: *the ip of the server*
Agent name: *whatever you want to call it*

<img src="https://i.imgur.com/pu7dSvC.png" alt="Wazuh Deploy Agent Step 2">

And you should see some commands down below
We copy that and use Powershell in order to install the agent
Make sure you run Powershell as Administrator

<img src="https://i.imgur.com/szAFpz4.png" alt="Wazuh Deploy Agent Step 3">

# Deploy Agent on Wazuh using Linux

# Deploy Agent on Wazuh using macOS


