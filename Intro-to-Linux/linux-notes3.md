# 🐧 Linux - Day 3 Summary

> 📅 **Date:** June 24, 2025  


---

## 📂 File System Hierarchy 

The Linux operating system is structured in a tree-like hierarchy and is documented in the **Filesystem Hierarchy Standard (FHS)**.

| 📁 Directory | 📘 Description |
|-------------|----------------|
| `/`         | Root directory – the base of all directories. |
| `/bin`      | Essential binary commands (e.g., `ls`, `cp`, `mv`). |
| `/boot`     | Bootloader, kernel, and files required to boot Linux. |
| `/dev`      | Device files to access hardware (e.g., `/dev/sda`). |
| `/etc`      | System-wide config files (network, users, services). |
| `/home`     | User directories (e.g., `/home/yana`). |
| `/lib`      | Shared libraries needed at system startup. |
| `/media`    | Mount point for USBs and external media. |
| `/mnt`      | Temporary mount points. |
| `/opt`      | Optional software packages. |
| `/root`     | Root user's home directory. |
| `/sbin`     | System admin commands (e.g., `reboot`, `shutdown`). |
| `/tmp`      | Temporary files. Emptied on reboot. |
| `/usr`      | User programs, man pages, libraries. |
| `/var`      | Variable data (logs, mail, web cache, etc). |

---

## 👤 User Management – Essential Commands

> Manage users, groups, passwords, and permissions.

| 🔧 Command  | 📘 Description |
|------------|----------------|
| `sudo`     | Execute a command as another user (usually root). |
| `su`       | Switch user (`su -` for full environment). |
| `useradd`  | Add a new user account. |
| `userdel`  | Delete user account and home directory. |
| `usermod`  | Modify existing user (e.g., change shell, group). |
| `addgroup` | Add a new group to the system. |
| `delgroup` | Remove a group. |
| `passwd`   | Change a user's password. |

📝 Tip: Combine `usermod -aG sudo yana` to add Yana to the sudoers group.

---

## 📌 Goal of This Part:
To give you strong foundational knowledge of:

How Linux organizes its system

How users and permissions are managed
