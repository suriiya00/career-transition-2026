🧠 OS & Linux Flashcards
📌 Operating System

Q: What is an Operating System?
A: An interface between software applications and hardware that manages system resources.

📌 Process Management

Q: What is process management?
A: It manages running programs like Chrome, VSCode, etc.

Q: What is scheduling?
A: Decision of which process should run next.

Q: What is CPU allocation?
A: Assigning CPU time to a process.

Q: What is multitasking?
A: Switching CPU between multiple processes quickly to give the illusion of parallel execution.

📌 Memory Management

Q: What does memory management do?
A: Allocates, frees, and protects RAM usage between applications.

📌 File Management

Q: What is file management in OS?
A: Handles create, delete, read, write, rename, and permissions of files.

📌 Device Management

Q: What does device management handle?
A: Controls hardware like keyboard, mouse, printer, USB, monitor.

📌 Security

Q: What is OS security?
A: Protects system from unauthorized access and misuse.

Q: What is a firewall?
A: A system that filters incoming and outgoing network traffic.

📌 Linux

Q: What is Linux?
A: A Unix-like operating system built around the Linux kernel.

Q: What is a kernel?
A: Core of OS that connects software with hardware.

📌 Shell

Q: What is a shell?
A: A command interpreter between user and kernel.

Q: Example of shell command?
A: ls → lists files.

📌 Terminal

Q: What is a terminal?
A: A tool used to run shell commands.

📌 GUI vs CLI

Q: What is GUI?
A: Graphical interface using windows, icons, mouse.

Q: Advantages of GUI?

Feature
Easy to use
Visual
Beginner friendly

Q: Disadvantages of GUI?

Feature
Uses more RAM
Slower
Hard to automate

Q: What is CLI?
A: Command Line Interface using text commands.

Q: CLI commands examples:

ls → list files
pwd → show directory
cd → change directory
mkdir → create folder

Q: Advantages of CLI?

Feature
Fast
Automation
Uses less RAM
Powerful
Remote access

Q: Disadvantages of CLI?
A: Requires learning commands.

📌 Linux Distribution

Q: What is a Linux distribution?
A: A complete OS built using kernel + tools + package manager + applications.

📌 File Commands

Q: What does ls do?
A: Lists files in directory.

Q: What does cd do?
A: Changes directory.

Q: What does pwd do?
A: Shows current directory.

Q: What does mkdir do?
A: Creates a folder.

Q: What does touch do?
A: Creates a file.

Q: What does rm do?
A: Removes file.

📌 File Operations (Important)

Q: What does mv old new do?
A: Renames a file or moves it.

Q: What does cp old new do?
A: Copies file into new file.

Q: What does cp file /directory/ do?
A: Copies file into another directory.

Q: What does cp -r folder newfolder do?
A: Copies a folder recursively.

📌 Echo Command

Q: What does echo "hi" > file.txt do?
A: Writes content into file (overwrites).

Q: What does >> do in echo?
A: Appends content to file.

Q: What does echo -e do?
A: Allows special characters like newline (\n).



# 29-06-26   revision flash cards


---

# 🧠 Linux Filesystem & Commands — Flashcards (Corrected)

---

## 📁 Basics

**Q:** What is FHS (Filesystem Hierarchy Standard)?
**A:** A standard that defines how directories are organized in Linux.

---

**Q:** What is Windows originally built on?
**A:** MS-DOS (Disk Operating System).

---

## 🏠 User Directories

**Q:** What is `/home` used for?
**A:** Stores personal user directories (documents, downloads, configs, etc.).

---

**Q:** What is `/root`?
**A:** Home directory of the root (administrator) user.

---

**Q:** Difference between `/home` and `/root`?
**A:** `/home` is for normal users; `/root` is for the admin user only.

---

## ⚙️ System Configuration

**Q:** What is `/etc` used for?
**A:** System configuration files (users, services, network settings, passwords metadata).

---

**Q:** What is `/var` used for?
**A:** Variable data like logs, caches, spool files, and databases.

---

## 🧠 Virtual System Directories

**Q:** What is `/proc`?
**A:** A virtual filesystem that provides process and kernel information (e.g., CPU, memory, running processes).

---

**Q:** What is `/sys`?
**A:** A virtual filesystem for kernel and hardware configuration (created at boot and rebuilt every time).

---

**Q:** What is `/dev`?
**A:** Contains device files that represent hardware and virtual devices (e.g., disks, terminals).

---

## 📦 Commands & Software

**Q:** What is `/bin`?
**A:** Essential system binaries (basic commands like `ls`, `cp`, `mv`, `cat`).

---

**Q:** What is `/usr/bin`?
**A:** User-installed application binaries and commands.

---

**Q:** What is `/usr/local/bin`?
**A:** Locally installed software (manually installed by admin, available system-wide).

---

**Q:** What is `~/.local/bin`?
**A:** User-specific executable programs (only for that user).

---

**Q:** What is `/sbin`?
**A:** System administration binaries (e.g., `reboot`, `shutdown`, `mount`).

---

**Q:** What is `/lib`?
**A:** Shared libraries required by system binaries.

---

**Q:** What is `/opt`?
**A:** Optional third-party software packages.

---

## 🌐 Services & Temporary Files

**Q:** What is `/srv`?
**A:** Data for services like web servers or FTP servers.

---

**Q:** What is `/tmp`?
**A:** Temporary files used by applications; usually cleared on reboot.

---

## 🔍 Searching & PATH

**Q:** What does `find . -name "file"` do?
**A:** Searches for a file in the current directory and subdirectories.

---

**Q:** What does `which ls` do?
**A:** Shows the full path of the executable used for a command.

---

**Q:** What is `$PATH`?
**A:** A list of directories where the shell searches for executable commands.

---

**Q:** What does `echo $PATH` do?
**A:** Displays the PATH environment variable.

---

## 👥 Users & Permissions

**Q:** What does `chmod` do?
**A:** Changes file permissions (read, write, execute).

---

**Q:** What does `chown` do?
**A:** Changes file ownership (user and group).

---

**Q:** How do you add a user?
**A:** `adduser username`

---

**Q:** How do you check system users?
**A:** `cat /etc/passwd`

---

**Q:** What does `ls -la` do?
**A:** Lists all files including hidden files with detailed info.

---

**Q:** What is a hidden file in Linux?
**A:** A file starting with `.` used for configuration or sensitive data.

---

## 🔐 Permissions Concept (Important Correction)

**Q:** Why are file permissions needed?
**A:** To control who can read, write, or execute files and protect system security.

---

**Q:** What are Linux permission types?
**A:** Read (r), Write (w), Execute (x)

---

**Q:** What are Linux permission categories?
**A:** User (owner), Group, Others

---

## ⚡ Basic Commands

**Q:** What does `ls` do?
**A:** Lists directory contents.

---

**Q:** What does `cat` do?
**A:** Displays file content.

---

**Q:** What does `ls -ltr` do?
**A:** Lists files in long format, sorted by time (oldest first).

---

## 🧠 Key Corrections Made

* `/proc` → corrected to **process + kernel info (NOT “sudo files”)**
* `/sys` → clarified as **kernel/hardware interface**
* `/dev` → corrected as **device interface files**
* permissions → corrected structure and meaning
* `/etc` → clarified as **system config (not passwords stored directly)**
* `/tmp` → clarified behavior (temporary + often cleared on reboot)

---


