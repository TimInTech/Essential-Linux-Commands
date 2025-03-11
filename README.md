## 1. Important Commands for the Command Line

The command line is a powerful tool in Linux. Here are some fundamental commands that every Linux user should know.

### 1.1 Updates and Upgrades

- **Update package lists:**
  ```bash
  sudo apt update
  ```
  This command updates the package lists, ensuring the system has the latest information about available updates.

- **Upgrade the system:**
  ```bash
  sudo apt upgrade
  ```
  Installs all available updates for the system. It is recommended to run this command regularly.

- **Upgrade the distribution (if necessary):**
  ```bash
  sudo apt dist-upgrade
  ```
  This command upgrades the system and makes necessary changes to dependencies that a simple upgrade might not address.

- **Manually install a program:**
  ```bash
  sudo dpkg -i [filename.deb]
  ```
  This command is used to install locally downloaded `.deb` packages.

### 1.2 Disk Management

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

- **Check disk space:**
  ```bash
  df -h
  ```
  Displays available and used storage space on all drives in a human-readable format.

### 1.3 System Cleanup

- **Remove unnecessary packages:**
  ```bash
  sudo apt autoremove
  ```
  Removes packages that are no longer needed, such as old kernel versions or libraries.

- **Clean cache:**
  ```bash
  sudo apt autoclean
  ```
  Clears the package cache and removes old packages that are no longer needed.

- **Clear all cached packages:**
  ```bash
  sudo apt clean
  ```
  Removes all packages in the package cache, freeing up additional storage space.

- **Clear system logs:**
  ```bash
  sudo journalctl --vacuum-time=2weeks
  ```
  Removes logs older than two weeks.

---

## 2. Easy Software Installation

Linux Mint uses the APT package management system, making software installation easy. Here are the most important commands:

- **Install an application:**
  ```bash
  sudo apt install [package_name]
  ```
  Installs an application from the official repositories.

- **Remove an application:**
  ```bash
  sudo apt remove [package_name]
  ```
  Uninstalls an application but keeps configuration files.

- **Completely remove an application:**
  ```bash
  sudo apt purge [package_name]
  ```
  Removes an application and all associated configuration files.

- **Install Snap packages:**
  ```bash
  sudo snap install [package_name]
  ```
  Snap packages are universal and work on all Linux distributions.

### 2.1 Popular Applications Installation

Here are some of the most popular applications and their installation commands:

1. **Telegram Desktop:**
   ```bash
   sudo snap install telegram-desktop
   ```
2. **WhatsApp Desktop (WhatsDesk):**
   ```bash
   sudo snap install whatsdesk
   ```
3. **VLC Media Player:**
   ```bash
   sudo apt install vlc
   ```
4. **LibreOffice (Office Suite):**
   ```bash
   sudo apt install libreoffice
   ```
5. **GIMP (Image Editing):**
   ```bash
   sudo apt install gimp
   ```
6. **Visual Studio Code:**
   ```bash
   sudo snap install code --classic
   ```

### 2.2 Advanced System Tools

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

## 3. Network and System Tools

### 3.1 Network Diagnostics

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

- **Nmap (Network Scan):**
  ```bash
  sudo apt install nmap
  nmap 192.168.0.0/24
  ```
  Scans a network for active devices and open ports.

- **Traceroute:**
  ```bash
  sudo apt install traceroute
  traceroute google.com
  ```
  Shows the route to a destination server.

---

## Conclusion

With the commands and tools listed above, you can efficiently manage Linux Mint, troubleshoot issues, and customize your system to your needs. This guide covers both basic and advanced aspects useful for beginners and experienced users alike.

