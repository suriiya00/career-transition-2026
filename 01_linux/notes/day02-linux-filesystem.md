````md
# Linux System vs Windows (Very Early Concept)

At the very beginning:
- Windows was installed on top of DOS (Disk Operating System)

---

# Linux Filesystem Hierarchy (FHS)

Linux System
│
├── /home   → People's houses
├── /etc    → Government office (configuration)
├── /var    → Warehouse (logs, databases)
├── /usr    → Shopping mall (applications)
├── /lib    → Power station (libraries)
└── /bin    → Toolbox (essential tools)

---

# Key Linux Directories Explained

## /home
It contains user-specific directories and data like:
- Documents
- Downloads
- Personal program files

👉 These are only for specific users, not all system users.

---

## /bin
- “bin” means binary
- Contains essential shell/system commands

Example:
- `ls`, `cp`, `mv`, `cat`

---

## /usr/bin
- Contains installed programs and external packages

---

## /usr/local/bin
- Used for manually installed software (by administrator)

Example:
- Node.js installed manually

👉 Programs here are available to all users

---

## ~/.local/bin
- User-specific binaries
- Only accessible to that particular user

---

## PATH concept
- When you type a command, the system searches directories in:

```bash
echo $PATH
````

* It finds executables inside `/bin`, `/usr/bin`, etc.

To check where a command is located:

```bash
which ls
```

---

## /root

* Private home directory of the administrator (root user)
* Has full system control

👉 Not the entire system, just one special user directory

---

## /etc

* Contains configuration files
* Examples:

  * User authentication
  * Password settings
  * Service configurations

---

## /var

* Variable data storage
* Includes:

  * Logs
  * Cache
  * Databases

---

## /sbin

(system binaries)

* Contains system administration commands:

  * reboot
  * shutdown
  * mount

---

## /lib

* Contains libraries required by `/bin` and `/sbin`
* Provides shared functions for programs

---

## /opt

* Optional software packages

---

## /proc

* Virtual filesystem
* Provides process and system information

Example:

```bash
cat /proc/cpuinfo
```

---

## /srv

* Service-related data
* Used by web servers and network services
* Improves structure and security

---

## /sys

* is a virtual filesystem that exposes information about the kernel, hardware devices, and drivers. It also allows certain hardware settings to be configured.

* Kernel-related system information
* Can change system settings (hardware, GPU, etc.)
* Recreated every reboot

---

## /tmp

* Temporary files
* Used by running applications
* Cleared automatically in many systems

---

# File Permissions in Linux

Permissions ensure system safety and prevent unauthorized changes.

## Why permissions are needed?

* Prevent accidental deletion of important files
* Control access between users (developer, QA, etc.)

---

## User management commands

```bash
adduser <username>
```

Example users:

* dev
* qa

---

## Check users

```bash
cat /etc/passwd
```

---

## File permissions

Create a file:

```bash
touch /tmp/example.sh
```

Check permissions:

```bash
ls -ltr
```

---

## chmod (change permissions)

Example:

```bash
chmod o=example.sh
```

Permission structure:

```
-   rw   -   rw   -   r   --
|    |       |        |
dir  usr     grp    others
```

---

## Key commands summary

### find command

```bash
find . -name "filename"
```

Finds file paths in directory tree.

---

# Quick Q&A Section

## What is /etc?

Directory containing:

* Users
* Groups
* Password/authentication files
* System configurations

---

## What is /var?

* Stores variable data like logs and cache

---

## What is /proc?

* Virtual system files
* Provides CPU, process, kernel info

---

## What is /dev?

* Contains device files

---

## What is /tmp?

* Temporary files for running processes

---

## Difference between /home and /root?

* `/home`: Individual user directories
* `/root`: Administrator (root user) home directory with full system control

---

## What does chmod do?

* Changes file permissions (read/write/execute)

---

## What does chown do?

* Changes file ownership

---

## Difference between ls and ls -la?

* `ls` → shows file list
* `ls -la` → shows all files including hidden ones

---

## What is a hidden file?

* Hidden files are files or folders whose names start with a dot (.). They are hidden from normal directory listings to reduce clutter. Many configuration files (such as .bashrc or .gitconfig) are hidden.

```

---
```
