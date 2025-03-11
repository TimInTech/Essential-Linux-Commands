# 📖 Essential Linux System Commands & Guides

Welcome to the **Essential Linux System Commands & Guides** repository! 🚀  
This repository contains an extensive collection of Linux commands for efficient system management, troubleshooting, and automation.

## 📌 Features
✅ Covers **system updates, disk management, software installation, networking, and cleanup tasks**  
✅ Beginner-friendly with clear explanations and command examples  
✅ Useful for **Sysadmins, DevOps, and Linux enthusiasts**  

---

## 🛠 Key Sections

### 🔹 System Updates & Upgrades
Manage updates and keep your system secure.

- **Update package lists:**
  ```bash
  sudo apt update
  ```
  This command refreshes the package lists, ensuring the system has the latest information about available updates.

- **Upgrade all installed packages:**
  ```bash
  sudo apt upgrade -y
  ```
  Installs all available updates for the system. It is recommended to run this command regularly.

- **Upgrade the distribution (if necessary):**
  ```bash
  sudo apt dist-upgrade
  ```
  This command upgrades the system and makes necessary changes to dependencies that a simple upgrade might not address.

- **Manually install a `.deb` package:**
  ```bash
  sudo dpkg -i [filename.deb]
  ```
  Replace `[filename.deb]` with the actual file name. This command is used to install locally downloaded `.deb` packages.

---

### 🔹 Disk Management

- **List attached drives:**
  ```bash
  lsblk
  ```
  Displays all available drives and partitions. Very useful for seeing which devices are connected.

- **Check and repair a disk:**
  ```bash
  sudo fsck /dev/sdX
  ```
  Replace `sdX` with the drive name. This command checks the file system for errors and repairs them if possible.

- **Check disk space usage:**
  ```bash
  df -h
  ```
  Displays available and used storage space on all drives in a human-readable format.

---

### 🔹 System Maintenance & Cleanup

- **Remove unnecessary packages:**
  ```bash
  sudo apt autoremove
  ```
  Removes packages that are no longer needed, such as old kernel versions or libraries.

- **Clean package cache:**
  ```bash
  sudo apt autoclean
  ```
  Deletes old package files that are no longer required.

- **Clear all cached packages:**
  ```bash
  sudo apt clean
  ```
  Completely removes all stored package files from the cache.

- **Delete old system logs:**
  ```bash
  sudo journalctl --vacuum-time=2weeks
  ```
  Removes logs older than two weeks to free up disk space.

---

### 🔹 Network Diagnostics

- **Show IP addresses:**
  ```bash
  ip a
  ```
  Displays all active network adapters and their configurations.

- **Perform a ping test:**
  ```bash
  ping google.com
  ```
  Checks the connection to a target address.

- **Scan a network for devices using Nmap:**
  ```bash
  sudo apt install nmap
  nmap 192.168.1.0/24
  ```
  Scans a network for active devices and open ports.

- **Check route to a destination server:**
  ```bash
  sudo apt install traceroute
  traceroute google.com
  ```
  Shows the path that network packets take to reach a remote host.

---

### 🔹 Software Installation

- **Install a package using APT:**
  ```bash
  sudo apt install [package_name]
  ```
  Installs an application from the official repositories.

- **Remove a package:**
  ```bash
  sudo apt remove [package_name]
  ```
  Uninstalls an application but keeps configuration files.

- **Completely remove a package and its config files:**
  ```bash
  sudo apt purge [package_name]
  ```

- **Install Snap packages:**
  ```bash
  sudo snap install [package_name]
  ```
  Snap packages are universal and work on all Linux distributions.

---

### 🔹 Advanced System Tools

- **Timeshift (System Backups):**
  ```bash
  sudo apt install timeshift
  ```
  Allows creating system snapshots for easy recovery.

- **Htop (System Monitoring):**
  ```bash
  sudo apt install htop
  ```
  An interactive tool for monitoring system resources like CPU and memory usage.

- **BleachBit (System Cleanup):**
  ```bash
  sudo apt install bleachbit
  ```
  Removes temporary files and frees up storage space.

---

## 📬 Contact
💬 **Email:** gummiflip@outlook.de  
🌍 **GitHub:** [TimInTech](https://github.com/TimInTech)

