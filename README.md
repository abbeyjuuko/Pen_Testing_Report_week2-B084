# Pen_Testing_Report_week2-B084

# My-week-2-Cyber-Security-Assignment BO84
using various tools to carry out Footprintingg and recon
<div align="center">

# 🔐 Cybersecurity Lab Environment Setup

**Building an isolated virtual lab for penetration testing and ethical hacking practice**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.2-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Virtualization-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali%20Linux-404040?style=flat-square&labelColor=C00000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Abbey%20Juuko%20CEH-C00000?style=flat-square" />
</p>

---

## 📌 Project Overview

This project focuses on using footprinting tools a **virtual cybersecurity and penetration-testing laboratory** using VirtualBox,Kali Linux and zenmap.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

---


## 🎯 Objectives

The main objectives of this project are to:

- Open kali linux.
- Open the terminal.
- Type various footprinting commands.
- Configure network connectivity for Kali Linux.
- Take a clean VM snapshots for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.

---

## 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

Its main use is to carry out footprinting and recon using commands such as:

- Whois 
- whatweb
- nslookup
- curl -I
- watw00f
- dns recon
- zenmap

⚠️ **Important:** This laboratory must only be used for systems that you own or have explicit permission to test. Do not use the lab or its tools to attack unauthorized systems.

---

## 🏗️ Lab Architecture

![](1-screenshot-title-image.png)


Additional target machines can be added to the same virtual network in future projects.

---

## ⚙️ Lab Configuration

| 🧩 Component       | ⚙️ Configuration   |
| ------------------ | ------------------  |
| 🖥️ Host OS         | Windows 11         |
| 🧠 Host RAM        | 16GB               |
| ⚡ Processor       | AMD Ryzen 5 865HS      |
| 🧰 Hypervisor      | VirtualBox 7.2  |
| 🐉 Security OS     | Kali Linux 2026.2  |
| 🧠 Kali RAM        | 6050 MB            |
| 🌐 Virtual Network | NAT Network        |
| 📡 Network Address | 10.0.0.0/24        |
| 🐧 Kali IP Address | 10.0.0.2/24        |
| 🚪 Default Gateway | 10.0.0.1           |
| 🌍 DNS Server      | 8.8.8.8            |
| 🔮 Future VM Range | 10.0.0.3–10.0.0.99 |

---

# 🪜 Lab Setup Procedure

## Step 1. Open kali terminal;

---

## Step 2. Make sure the VM can acess internet



---

## Step 3. type whois in the terminal:;

## Screenshot of the whois command

![](<img width="752" height="631" alt="image" src="https://github.com/user-attachments/assets/07ac44fc-8d63-4865-9f16-6c87b1710ed5" />
png)

A **whois command**

This will reveal the registrar, registration and expiry dates and the name servers within the labthe lab.



## Step 4. whatweb command

## Screenshot of the whatweb command

The whatweb command exposes the exact softwareand versions (here word press 7.1.4 and apache were used)

![](<img width="675" height="512" alt="image" src="https://github.com/user-attachments/assets/0afe0f4d-09a7-43e2-b27d-a83a9ef13de0" />





## Step 5. Type the nslookup command in the terminal

The Nslookup command turns a domain name into its real ip (192.232.216.135). Knowing an ip lets the attacker scan the server directly, look up other sites on the same ip and maps the target infrastructure.

## Screenshot of the ns lookup command

![](<img width="715" height="237" alt="image" src="https://github.com/user-attachments/assets/f7ee6c03-a0a7-4eb5-86ed-154b0a8378b2" />
)



## Step 6. Type in the Curl -I command

An attacker can use this in that the http headers leak the web server, caching stack and hidden end points

## Screenshot of the curl -I command

![]()

## Step 7 MY Windows 11 Setup

I downloaded my win 11 and configured it into the virtual box.

## Screenshot of win 11

![](my%20win%2011.png)

## Step 8. Win 11 Netwok setup in winthin the virtual box

## Screenhot of network setup of win 11

![](my%20win%2011%20network%20seup.png)


## Step 9.Setting up my Configured Android VM in virtual Box


 ## Screenshot of my Android VM.


![](setting%20up%20android%20vm.png)

## Step10. Setting up Network of the Android VM in the Virtual Box

## Screenshot of setting up th Network.

![](setting%20up%20android.png)


 




---

# 🔎 Lab Verification

| ✅ Test                        | 🧾 Command                      | 🎯 Expected Result              |
| ----------------------------- | ------------------------------- | ------------------------------- |
| 🌐 Check IP address           | `ip a`                          | Correct Kali IP displayed       |
| 📡 Test gateway               | `ping 10.0.0.1`                 | Successful replies              |
| 🌍 Test Internet connectivity | `ping 8.8.8.8`                  | Successful replies              |
| 🔎 Test DNS resolution        | `nslookup networkwalks.com`     | Domain resolves                 |
| 🧰 Verify Nmap                | `nmap --version`                | Nmap version displayed          |
| 🔄 Verify snapshot            | Restore snapshot and run `ip a` | Baseline configuration restored |

### Results


IP Address:
10.0.0.2/24

Gateway:
10.0.0.1

DNS:
8.8.8.8
```

---

# 🐞 Problems Encountered & Solutions

Documenting problems is an important part of the project.

## Problem 1. Internet Connectivity After Static IP Configuration

After manually configuring the IPv4 settings, Internet connectivity may fail depending on the Kali/NetworkManager configuration.

One workaround used during this lab was:

```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
```

The network connection was then restarted/rebooted and connectivity was tested again.

> **Important:** Network interface and connection names may differ between systems. Students should first identify their actual connection name before running an `nmcli` command.

---

## Problem 2. VirtualBox VT-x / Virtualization Error

The VM initially failed to start because hardware virtualization was disabled in the system firmware/BIOS.

The issue was resolved by:

1. Restarting the computer.
2. Entering BIOS/UEFI settings.
3. Enabling Intel VT-x / hardware virtualization.
4. Saving the configuration.
5. Restarting the computer.
6. Starting the Kali VM again.

After enabling virtualization, the VM started successfully.

## Problem 3. Android VM setup

The VM failed to install beacause of hardware virtualization and little base memory and limited cores.

The issue was resolved by:

1. Restarting the computer.
2. Maximizing the base memory to atleast 8060mb.
3. Increasing the processor cores to 6cores.


---

# 💡 What I Learned

Through this project, I learned how to create and configure a virtual environment for cybersecurity practice.

The most important concepts I learned include:

### 1. NAT vs NAT Network

A standard NAT configuration and a NAT Network serve different purposes.

A NAT Network allows multiple VMs connected to the same virtual network to communicate with one another while providing network address translation for external connectivity.

This makes it useful for building a multi-machine cybersecurity laboratory.

### 2. Virtual Machine Networking

I learned how VirtualBox virtual network adapters connect virtual machines to different types of networks and how network configuration affects communication between machines.

### 3. Static IP Configuration

I learned how to configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in Kali Linux.

### 4. VM Snapshots

I learned that a clean snapshot should be created **before performing risky or experimental activities**.

This provides a known-good recovery point for future cybersecurity exercises.

### 5. Documentation

I learned that documenting commands, configuration, screenshots, problems, and solutions is an important part of a professional cybersecurity project.

---

---

# 🔗 Tools & Resources

- **7-Zip:** [https://7-zip.org/download.html](https://7-zip.org/download.html)
- **VirtualBox:** [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
- **Kali Linux:** [https://kali.org/get-kali](https://kali.org/get-kali)
- **Win 11:** [https://www.microsoft.com/en-us/software-download/windows11]
- **Android X64:** [https://www.android-x86.org/download.html]

---

# 👤 Author

**ABBEY JUUKO**\
Cybersecurity Specialist B084D

LinkedIn: [www.linkedin.com/in/juuko-abbey-serwanga-4a72b6315)

---

## Project Information

**Program Name:** Cybersecurity at Networkwalks | **Week:** 01 | **Project:** Cybersecurity & Pentesting Lab Setup | **Repository:** GitHub
