Linux Essentials — Day 8

User Management, Ownership & Permissions

1. Linux User Types & Identity

Multi-User System: Linux allows multiple users to access the system simultaneously, tracking each via a unique UID (User ID).
Root User (UID 0): The superuser account with unrestricted, total control over the entire operating system.
Regular Users: Standard accounts created for daily tasks, with restricted access to system files.

2. Identity Verification Commands

whoami ➡️ Displays the username of the current active terminal session.
id ➡️ Prints the current user's UID, GID (Group ID), and the groups they belong to.
su [username] ➡️ Switches the current session to another user (Switch User).
sudo [command] ➡️ Executes a single command with root (administrator) privileges.

3. Managing Users and Groups

useradd ➡️ Creates a new regular user account on the system.
passwd ➡️ Sets or updates the password for a specific user.
userdel -r ➡️ Deletes a user account and permanently removes their home directory.
groupadd ➡️ Creates a new user group to manage collective permissions.

4. Understanding File Ownership

Every file/directory has three ownership tiers:
User (u) ➡️ The specific user account that owns the file.
Group (g) ➡️ The group of users that shares access to the file.
Other (o) ➡️ All other users on the system (everyone else).

5. Permission Types & Numeric Values

Read (r) ➡️ Value: 4. Allows viewing file content or listing directory files.
Write (w) ➡️ Value: 2. Allows modifying file content or creating/deleting files in a directory.
Execute (x) ➡️ Value: 1. Allows running files as scripts or entering directories using 'cd'.

6. Modifying Permissions & Ownership

chmod ➡️ Changes file/directory permissions using either symbolic (e.g., u+x) or numeric (e.g., 755) methods.
chown ➡️ Changes the owner and/or group of a file (e.g., chown john:developers file.txt).

🔄 Current Focus: Reviewing core security concepts and practice assigning permissions on the terminal.
