# Linux Essentials — Day 6
## Chapter 6: Command Line Basics

### 1. Terminal Symbols
* `~` ➡️ Home directory of the user.
* `$` ➡️ Regular user (limited access).
* `#` ➡️ Root user (full admin access).

### 2. Virtual Terminals (TTY)
* **What:** Isolated text-based terminals at the kernel level.
* **Limit:** Up to 8 virtual terminals.
* **Shortcut:** `Ctrl + Alt + F1` to `F7`. 
* **Note:** TTY7 or TTY8 is usually your desktop GUI.
* **Use:** Managing processes, editing text, and system debugging.

### 3. Command Paths (PATH Variable)
Linux uses environment variables to find where programs are stored:
* **Normal Users:** Apps are in `/bin`, `/usr/bin`, `/usr/local/bin`.
* **Root User:** Admin tools are in `/sbin`, `/usr/sbin`, `/usr/local/sbin`.

### 4. Core Commands
* `ls` ➡️ List files and folders.
* `free` ➡️ Show remaining RAM memory.
* `touch` ➡️ Create a new empty file.
* `ping` ➡️ Test network connection tool.
* `pwd` ➡️ Show current directory path.
* `echo` ➡️ Print text or variable values.
* `type` ➡️ Show the exact location of a command.
* `cat` ➡️ View text file content.
* `man` ➡️ Open command manual/help page.
* `history` ➡️ See all past commands.
* `history -c` ➡️ Clear all command history.
* **Tab Key:** Auto-completes commands and filenames.da
