# Linux Essentials — Day 5
## Chapter 5: Hardware & System Components

### 1. CPU & Motherboard Architecture
* **Intel vs AMD:** The two main CPU manufacturers supported by Linux.
* **CPU Bit Depth:** Determines how much data a CPU can process per clock cycle.
  * **32-bit (x86):** Limited to a maximum of 4GB RAM.
  * **64-bit (x86_64 / amd64):** Modern standard, handles massive memory limits.
* **Motherboard:** The central nervous system of the computer.
  * **Slots:** Expansion ports on the motherboard (PCIe for GPUs, RAM slots).
  * **Form Factors:** Different sizes based on needs (e.g., ATX, Micro-ATX, Mini-ITX).
* **Power Supply (PSU):** Converts AC electricity (wall outlet) to DC electricity (used by PC components).

### 2. Storage, Partitions & File Systems
* **Sector:** The smallest physical unit on a hard drive (usually 512 bytes or 4KB).
* **The "C:" Drive History:** Windows uses `C:` because `A:` and `B:` were historically reserved for floppy disks.
* **File System Hierarchy:** * **Windows:** Uses separate roots for each drive (`C:\`, `D:\`).
  * **Linux:** Uses a single unified tree starting at the root directory (`/`).
* **MBR vs GPT:**
  * **MBR (Old):** Supports up to 4 primary partitions and max 2TB disk size.
  * **GPT (Modern):** Supports up to 128 partitions and has no practical size limits.
* **SWAP Memory:** A designated area on the disk used as virtual RAM when physical RAM is full.
* **Linux File Systems:** **ext3** and the modern **ext4** are the most popular native file systems.

### 3. Display & Drivers
* **CLI vs GUI:** For every graphical tool in Linux, a text-based (CLI) tool always exists.
* **X11 vs Wayland:** Display server protocols. X11/Xorg is the legacy system; **Wayland** is the modern, faster, and more secure successor.
* **Video Cables:** Legacy analog (VGA) vs modern digital (HDMI, DisplayPort).
* **Drivers:** Unlike Windows (where you install drivers manually), most Linux drivers are built directly into the Linux Kernel.

### 4. Basic Hardware Discovery Commands
Run these commands in the terminal to inspect your system:
* `lscpu` ➡️ Display CPU architecture details.
* `lsblk` ➡️ List all block storage devices and partitions.
* `lspci` ➡️ List all PCI devices (Graphics cards, Wi-Fi network cards).
* `lsusb` ➡️ List all connected USB devices.
* `free -m` ➡️ Show RAM usage in Megabytes.

### Challenges:
1. Run `lscpu` and check if your system is running a 64-bit kernel.
2. Run `free -m` to see how much SWAP space is configured on your Linux Mint machine.
