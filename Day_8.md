# 📑 Day 8: User Management, Ownership & Permissions

Welcome to Day 8! Today's study focuses on how Linux manages security, system users, groups, and file permissions. This is a crucial topic for the LPI Linux Essentials exam.

---

## 1️⃣ Linux User Types & Identity

Linux is a multi-user operating system. Every process and file is owned by a specific user.
* **Root User (`UID 0`):** The superuser or system administrator. It has unrestricted access to the entire system.
* **System Users:** Accounts used by the OS to run background services (e.g., `httpd`, `sshd`). They usually do not have login shells.
* **Regular Users:** Standard accounts created for actual people to perform daily tasks.

### 🔍 Key Identity Commands
* `whoami` : Displays the username of the current active session.
* `id` : Shows the current user's UID (User ID), GID (Group ID), and the groups they belong to.
* `su [username]` : Switch User. Allows you to switch to another user account (defaults to root if no user is specified).
* `sudo [command]` : Superuser Do. Executes a single command with root privileges.

---

## 2️⃣ Managing Users and Groups

Administrators use specific commands to maintain users and groups on the system.

| Command | Function & Description |
| :--- | :--- |
| `useradd [name]` | Creates a new regular user account. |
| `passwd [name]` | Sets or changes the password for a specific user. |
| `userdel -r [name]` | Deletes a user account along with their home directory (`-r`). |
| `groupadd [name]` | Creates a new user group for organizing permissions. |

---

## 3️⃣ Understanding File Ownership & Permissions

Every file and directory in Linux has three tiers of ownership:
1. **User (u):** The individual account that owns the file.
2. **Group (g):** The group of users that shares access to the file.
3. **Other (o):** Anyone else on the system who is not the owner or part of the group.

When you run `ls -l`, you see a 10-character permission string (e.g., `-rwxr-xr--`):
* First character indicates type: `-` for a regular file, `d` for a directory.
* Next 3 characters: **User** permissions.
* Next 3 characters: **Group** permissions.
* Last 3 characters: **Other** permissions.

### 🛑 Permission Types
* **Read (r):** Ability to view file content or list directory contents. (Value = `4`)
* **Write (w):** Ability to modify file content or add/delete files in a directory. (Value = `2`)
* **Execute (x):** Ability to run a file as a program or enter a directory using `cd`. (Value = `1`)

---

## 4️⃣ Modifying Permissions & Ownership

### 🔐 The `chmod` Command (Change Mode)
Used to alter file permissions. It can be done in two ways:
* **Symbolic Method:** `chmod u+x file.txt` (Adds execute permission for the owner).
* **Absolute (Numeric) Method:** Uses octal numbers.
```bash
  chmod 755 script.sh
  # 7 (rwx) for User, 5 (r-x) for Group, 5 (r-x) for Other
