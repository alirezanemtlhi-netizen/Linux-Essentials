# Linux Essentials — Day 7
## System Installation, PMS, Help Tools & Network Basics

### 1. OS Installation & Dual-Booting
* **Dual-Boot System:** Installing two operating systems (e.g., Linux Mint and Windows) on the same hard drive, allowing the user to choose which one to boot at startup.
* **GRUB Bootloader:** The software that loads up first and lets you select between your Linux or Windows OS during a dual-boot start.

### 2. Desktop Environments (DE) & PMS
* **Desktop Environments:** The graphical user interface (GUI) of Linux (e.g., Cinnamon, MATE, XFCE). They differ in look, feel, and resource (RAM/CPU) consumption.
* **PMS (Package Management System):** The software utility responsible for installing, updating, configuring, and removing software packages (e.g., `APT` for Debian/Mint, `RPM` for Red Hat).

### 3. Directory Navigation & File Management
* `cd ..` ➡️ Moves one level up into the parent directory.
* `pwd` ➡️ Prints the current absolute working directory path (Print Working Directory).
* `ls -a` / `ls -al` ➡️ Lists all files, including hidden files (those starting with a `.`), with detailed attributes.
* `touch` ➡️ Creates a new empty file or updates timestamps.
* `mkdir` ➡️ Creates a new directory (Make Directory).
* `cat` ➡️ Outputs the content of a file directly to the terminal (Concatenate).
* `rm -r` ➡️ Recursively deletes a directory and all of its contents.

### 4. Integrated Help Systems
* `--help` ➡️ Displays a quick, compact summary of a command's options.
* `man` ➡️ Opens the extensive, built-in reference manual for a command.
* `whatis` ➡️ Provides a very brief, one-line description of what a command does.
* `makewhatis` ➡️ Updates the internal manual page database (mandb).
* `apropos` ➡️ Searches the manual page descriptions for specific keywords.

### 5. Client-Side Network Basics & Protocols
Essential tools and concepts used to check and troubleshoot client-side network connections:
* **SSH (Secure Shell):** A secure, encrypted network protocol used to connect to remote servers (Port 22).
* **Telnet:** An older, unencrypted protocol that transmits data and credentials in plain text (highly insecure).
* `ping` ➡️ Tests network connectivity to a specific host or IP address.
* `ip a` / `ifconfig` ➡️ Displays the system's active network interfaces and IP addresses.

### 6. Variables & Globbing
* **Shell Variables:** Storing values in the temporary RAM memory. They must follow strict naming conventions: only alphanumeric characters and underscores (`_`) are allowed, special characters are forbidden, and they cannot contain spaces.
* **Globbing:** Using wildcard characters (like `*`) to perform pattern matching and filter groups of files (e.g., `ls *.txt`).

---
🔄 **Current Focus:** Pausing new topics to review all foundations from Day 1 onward to build a rock-solid base.
