Operating System (OS) Basics

OS - It is nothing but a interface which acts / communicate in between the software application and hadware as an intermidate.

Main Functionalities of OS
1. Process Management

Managing the running programs which is called Process.

Example: Running applications like Chrome, VSCode, etc.

Note:

The OS itself decides which program runs first
CPU allocation → It is the thing that gives CPU to the process
Scheduling → It is the thing that selects among 4 processes what to run
Multitasking → It is the keeping on shifting the CPU among the processes at the same interval of time. To imagine all processes working at a time

Summary:
Scheduling is the decision-making step, CPU allocation is the action of handing over the CPU, and multitasking is the overall behavior produced by repeatedly scheduling and allocating the CPU among processes.

2. Memory Management

It is the one how manages RAM (Random Access Memory) and does things like:

Allocation of memory
Free unused memory
Prevent applications from interfering with each other
3. File Management

It manages file operations like:

Creation
Deleting
Rename
Read
Write
Permissions
4. Device Management

Controls hardware devices like:

Keyboard
Mouse
Printer
Monitor
USB drives
5. Security

Protecting the computer, its data, and its resources from unauthorized access, misuse, or attacks.

Provides:

User authentication
Passwords
Permissions
Encryption
Firewall
Notes:
Reason keeps sensitive data confidential
Firewall acts like a watchman to the network
It checks incoming and outgoing data and decides whether to:
✅ Allow safe traffic
❌ Block suspicious or unauthorized traffic


What is Linux?

Linux is an open-source kernel that serves as the core of many operating systems such as Ubuntu, Debian, Fedora, and CentOS.

Note:
Kernel is the most important thing which acts as central part. It is the one that sends responses from hardware to software.

Linux is used by most of the companies like:

Google
Amazon
Meta
Netflix
NVIDIA
Samsung
Intel
Oracle



Shell

A Shell is a command interpreter.

It accepts commands from the user and sends them to the Linux Kernel.

Example:

ls → show all files list

Popular shells:

bash
sh
Shell Responsibilities
Execute commands
Run scripts
Variables
Loops
Conditions
Pipes
Redirection
Terminal

It is the tool to use shell commands for executing, running, etc.

GUI vs CLI
GUI (Graphical User Interface)

Uses:

Windows
Icons
Mouse
Buttons
Advantages
Advantages
Easy to learn
User friendly
Visual
Disadvantages
Disadvantages
Consumes more RAM
Slower
Harder to automate
CLI (Command Line Interface)

Uses commands to interact:

ls → list files
pwd → print working directory
cd → change directory
mkdir → create folder
Advantages
Advantages
Very fast
Automation
Remote access
Powerful
Uses less RAM
Preferred by DevOps engineers
Disadvantages
Disadvantages
Requires learning commands
What is Linux Distribution?

It is a complete operating system built using:

Linux Kernel
GNU tools
Package manager
Desktop environment (optional)
Utilities and applications

A distribution packages everything needed to use Linux like Ubuntu, Debian, RedHat, CentOS, etc.

Linux Architecture
Linux Kernel
        │
 ┌──────┴──────────────┐
 │                     │
Debian Family      Red Hat Family
 │                     │
Ubuntu            Fedora
 │                     │
Linux Mint       RHEL
                 │
             CentOS Stream
Interview Summary
Operating System: Software that manages hardware and provides services for applications.
Linux: Open-source Unix-like operating system built around the Linux Kernel.
Why Linux?: Secure, stable, customizable, efficient, and dominant in servers, cloud, and DevOps.
Kernel: Core of the OS that manages hardware, memory, processes, and devices.
Shell: Command interpreter that translates user commands into actions for the kernel.
Terminal: Application used to interact with the shell.
GUI vs CLI: GUI is visual and beginner-friendly; CLI is faster, scriptable, and preferred for administration.
Linux Distribution: Complete OS combining kernel, tools, package manager, and apps.
Linux Commands Practice (28-06)
ls → list all files
cd → change directory
mkdir → create folder
pwd → present working directory
touch → create file
rm → remove file
File Operations

Rename file:

mv oldfile newfile

Copy file:

cp newcreatingfile creatingfile

Copy file to another directory:

cp newcreatingfile /home/workspace/career-transtion-2026/01_linux/pratice

Copy folder:

cp -r practice newpractice

Verbose copy with overwrite prompt:

cp -rv creatingfile project_backup
Echo Command

Write content:

echo "hi" > file.txt

Append content:

echo "hello" >> file.txt

Multiple lines:

echo -e "hi\nhello" > file.txt

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