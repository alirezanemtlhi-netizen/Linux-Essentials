# Linux Essentials — Day 7
## Chapter 7: System Installation, PMS & Network Basics

### 1. OS Installation & Dual-Booting
* **Dual-Boot System:** Installing two operating systems (e.g., Linux Mint and Windows) on the same hard drive, allowing the user to choose which one to boot at startup.
* **GRUB Bootloader:** The software that loads up first and lets you select between your Linux or Windows OS during a dual-boot start.

### 2. Desktop Environments (DE) & PMS
* **Desktop Environments:** The graphical user interface (GUI) of Linux (e.g., Cinnamon, MATE, XFCE). They differ in look, feel, and resource (RAM/CPU) consumption.
* **PMS (Package Management System):** The software utility responsible for installing, updating, configuring, and removing software packages (e.g., `APT` for Debian/Mint, `RPM` for Red Hat).

### 3. Basic Network Commands (Client-Side)
Essential CLI tools used to check and troubleshoot client-side network connections:
* `ping` ➡️ Tests network connectivity to a specific host or IP address.
* `ifconfig` / `ip a` ➡️ Displays the system's active network interfaces and IP addresses.
* `traceroute` / `tracepath` ➡️ Tracks the exact path/routers a data packet takes to reach a destination.
* `nslookup` / `dig` ➡️ Queries DNS servers to find the IP address of a domain name.

### Challenges:
1. Run `ip a` in your terminal to find your local IP address.
2. Try to ping a public DNS server (e.g., `ping 8.8.8.8`) to test your internet connection.
