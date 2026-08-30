# Linux for Beginners: A Practical Guide

![License](https://img.shields.io/badge/license-MIT-blue)
![Chapters](https://img.shields.io/badge/chapters-12%20of%2012-orange)
![Chapters](https://img.shields.io/badge/Chapters-Complete-brightgreen)
![Made with](https://img.shields.io/badge/made%20with-AI%20assisted%20research-blueviolet)

A complete, beginner-friendly guide to learning Linux from scratch. No prior experience needed. Whether you're a student, a future developer, or just someone curious about what's running behind most of the internet — this guide walks you through everything step by step, starting with the absolute basics and building up to real, practical skills.

---

## Table of Contents

| # | Chapter | Folder | Status |
|---|---------|--------|--------|
| 1 | [What Is Linux and Why Should You Learn It?](./Chapter-01-What-Is-Linux) | `Chapter-01-What-Is-Linux` | ✅ Published |
| 2 | [Navigating the Terminal: Your First Commands](./Chapter-02-Navigating-the-Terminal) | `Chapter-02-Navigating-the-Terminal` | ✅ Published |
| 3 | [Files & Directories: Creating, Moving, and Deleting](./Chapter-03-Files-and-Directories/) | `Chapter-03-Files-and-Directories` | ✅ Published |
| 4 | [Users, Permissions & the Root User](./Chapter-04-Users-and-Permissions) | `Chapter-04-Users-and-Permissions` | ✅ Published |
| 5 | [Installing & Managing Software with apt](./Chapter-05-Installing-and-Managing-Software/) | `Chapter-05-Installing-and-Managing-Software` | ✅ Published |
| 6 | [Text Editors: Reading and Editing Files in the Terminal](./Chapter-06-Text-Editors) | `Chapter-06-Text-Editors` | ✅ Published |
| 7 | [Processes & System Monitoring](./Chapter-07-Processes-and-System-Monitoring) | `Chapter-07-Processes-and-System-Monitoring` | ✅ Published |
| 8 | [Networking Basics: Connections, IPs & SSH](./Chapter-08-Networking-and-SSH) | `Chapter-08-Networking-and-SSH` | ✅ Published |
| 9 | [Shell Scripting: Automating Tasks with Bash](./Chapter-09-Shell-Scripting) | `Chapter-09-Shell-Scripting` | ✅ Published |
| 10 | [Disk Management & the Filesystem in Depth](./Chapter-10-Disk-Management-and-Filesystem) | `Chapter-10-Disk-Management-and-Filesystem` | ✅ Published |
| 11 | [System Logs, Services & systemd](./Chapter-11-System-Logs-Services-and-systemd) | `Chapter-11-System-Logs-Services-and-systemd` | ✅ Published |
| 12 | [What's Next: Linux in the Real World](./Chapter-12-Whats-Next) | `Chapter-12-Whats-Next` | ✅ Published |

---

## Why This Guide Exists

Most Linux tutorials either assume too much knowledge or throw a wall of commands at you without explaining why they matter. This guide takes a different approach. It starts with the big picture — what an operating system actually does, where Linux came from, and why it runs so much of the modern world — before slowly moving into hands-on terminal work.

By the end, you won't just know commands. You'll understand how Linux thinks.

---

## What You'll Learn

### ✅ Chapter 1 — What Is Linux and Why Should You Learn It?

This chapter lays the groundwork for everything else in the guide. It covers:

- The big picture of what an operating system actually does (resource management, hardware abstraction, and the user interface)
- A brief history of Linux — from Unix at Bell Labs in 1969, to Richard Stallman's GNU Project, to Linus Torvalds posting about his "hobby" operating system in 1991
- Linux vs. Windows vs. macOS: an honest, practical comparison across cost, customization, security, and use cases
- What a Linux distribution actually is, and the three major distro families: Debian/Ubuntu, Red Hat/Fedora, and Arch
- Desktop vs. terminal — why both matter and why the terminal holds Linux's real power
- The open-source philosophy behind Linux and why the GPL matters
- Setting up your first Linux environment using WSL2, a virtual machine, dual boot, or a live USB
- Your first login and first command, including a walkthrough of the GNOME desktop and your first terminal session
- A first look at the Linux filesystem, including the single-tree structure rooted at `/` and key directories like `/home`, `/etc`, and `/var`

📂 [Read Chapter 1 →](./Chapter-01-What-Is-Linux)

---

### ✅ Chapter 2 — Navigating the Terminal: Your First Commands

With the background from Chapter 1, this chapter puts your hands on the keyboard. It covers:

- What the shell actually is and the difference between `sh`, `bash`, and `zsh`
- Reading and understanding the shell prompt (`user@host:~$`)
- Navigating the filesystem with `pwd`, `ls`, and `cd`
- Absolute vs. relative paths — and why the distinction matters
- Useful shortcuts: `~`, `.`, `..`, `-`, and tab completion
- Getting help directly in the terminal with `man`, `--help`, and `whatis`
- Your first look at command structure: `command [options] [arguments]`
- Combining flags and reading manual pages without frustration

📂 [Read Chapter 2 →](./Chapter-02-Navigating-the-Terminal)

---

✅ **Chapter 3 — Files & Directories: Creating, Moving, and Deleting**
With navigation down, this chapter puts your hands on the filesystem itself. It covers:
- Creating files with `touch` and the `>` / `>>` redirection operators
- Creating directories with `mkdir` and nested paths with `mkdir -p`
- Viewing file contents with `cat`, `less`, `head`, and `tail -f` for live logs
- Copying files and directories with `cp` (and why `-i` is a good habit)
- Moving and renaming with `mv` — in one step or both at once
- Deleting with `rm` and `rmdir` — and why `rm -rf` deserves extreme caution
- Wildcards (`*`, `?`, `[]`) for acting on multiple files at once
- Finding files with `find` (live) and `locate` (fast index)

📂 [Read Chapter 3 →](Chapter-03-Files-and-Directories)

---

### ✅ **Chapter 4 — Users, Permissions & the Root User**
With the filesystem covered, this chapter tackles Linux's security model. It covers:
- Users, groups, UIDs, and GIDs — how Linux identifies who you are
- The root user and why you should almost never use it directly
- `sudo` — running privileged commands safely, and how the sudoers file works
- The permission model: read, write, execute for owner, group, and others
- Reading and decoding permission strings like `drwxr-xr-x`
- Changing permissions with `chmod` in both symbolic (`u+x`) and octal (`755`) mode
- Changing ownership with `chown` and `chgrp`
- Special permissions: setuid, setgid, and the sticky bit
- Managing users and groups from the command line

📂 [Read Chapter 4 →](./Chapter-04-Users-and-Permissions)

---

### ✅ **Chapter 5 — Installing & Managing Software with apt**
With permissions mastered, this chapter covers one of Linux's greatest practical strengths: its software management system. It covers:

- What a package manager is and why it's better than downloading installers
- How `apt` works: repositories, the package index, and Ubuntu's four repo components
- `sudo apt update` — refreshing the index (and what it does NOT do)
- Installing software with `apt install`, including useful flags like `-y` and `--dry-run`
- Removing software: `remove` vs `purge` vs `autoremove` — and when to use each
- Upgrading your entire system with two commands: `update` + `upgrade`
- Searching and inspecting packages with `apt search`, `apt show`, and `dpkg`
- `apt` vs `apt-get` — which to use in the terminal vs in scripts
- Adding PPAs and third-party repositories (e.g. Docker, Node.js)
- Installing from source with `configure / make / make install`, plus Snap, Flatpak, and AppImage

📂 [Read Chapter 5 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-05-Installing-Software-with-apt)

---

### ✅ **Chapter 6 — Text Editors: Reading and Editing Files in the Terminal**
With software management covered, this chapter tackles a skill you'll use every single day: editing files directly in the terminal. It covers:

- Why terminal text editors matter — especially for remote server work over SSH
- A comparison of available editors: nano, vim, neovim, emacs, and micro
- **nano** — the beginner-friendly editor: opening files, saving, searching, and the full shortcut reference
- **vim** — the powerful modal editor: understanding Normal, Insert, Visual, and Command modes
- The golden rule of vim: when in doubt, press `Esc`
- vim navigation, editing commands, search, and find-and-replace (`:%s/old/new/g`)
- Working with multiple files and split panes in vim
- Configuring vim with `~/.vimrc` — line numbers, syntax highlighting, tab settings
- Editing system config files safely: always back up before touching `/etc/fstab` or `sshd_config`
- Viewing files without editing: `cat`, `less`, `head`, `tail`, `grep`, `wc`

📂 [Read Chapter 6 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-06-Text-Editors)

---

### ✅ **Chapter 7 — Processes & System Monitoring**
With file editing covered, this chapter teaches you to see inside a running Linux system. It covers:

- What a process is: PID, PPID, owner, state, and the full process tree from PID 1
- Viewing processes with `ps aux` — reading every column and filtering with `grep`
- Live monitoring with `top` and the improved `htop`
- Sending signals to processes: `kill`, `killall`, and `pkill` — SIGTERM first, SIGKILL last
- Job control: running in background with `&`, pausing with `Ctrl+Z`, resuming with `bg` and `fg`
- Keeping processes alive after logout with `nohup` and persistent sessions with `screen`
- Monitoring memory with `free -h`, CPU/I/O with `vmstat` and `iostat`
- Disk usage: `df -h` for filesystem fullness, `du -sh` for directory sizes
- Understanding load average and what it means relative to your CPU core count

📂 [Read Chapter 7 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-07-Processes-and-System-Monitoring)

---

### ✅ **Chapter 8 — Networking Basics: Connections, IPs & SSH**
With system monitoring covered, this chapter connects your Linux machine to the world. It covers:

- How Linux networking works: interfaces, IP addresses, routes, ports, TCP vs UDP
- Inspecting network interfaces and routing with `ip addr show` and `ip route`
- Testing connectivity step by step with `ping` — loopback → gateway → internet → DNS
- Downloading files and interacting with APIs using `curl` and `wget`
- Checking open ports and connections with `ss -tlnp`
- DNS tools: `dig`, `nslookup`, and `host` — turning names into IPs
- Connecting to remote servers with `SSH` — the foundation of remote Linux work
- SSH keys: generating ED25519 key pairs, copying public keys, and setting correct permissions
- The `~/.ssh/config` file — shortcuts, port settings, and keepalive configuration
- Transferring files securely with `scp` and efficiently with `rsync`
- SSH tunnels and local/remote port forwarding
- Firewall management with `ufw` — allowing services and protecting your system

📂 [Read Chapter 8 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-08-Networking-and-SSH)

---

### ✅ **Chapter 9 — Shell Scripting: Automating Tasks with Bash**
With networking covered, this chapter brings everything together — writing scripts that automate repetitive tasks. It covers:

- What a shell script is and when to write one instead of typing commands manually
- The shebang line (`#!/bin/bash`), making scripts executable, and running them with `./`
- Variables, user input with `read`, and environment variables like `$USER`, `$HOME`, `$PWD`
- Command substitution `$()` and arithmetic with `$(( ))`
- Conditionals: `if`, `elif`, `else`, `fi` — with real decision-making examples
- Three families of test expressions: numeric (`-eq`, `-gt`), string (`==`, `-z`), file (`-f`, `-d`, `-x`)
- Loops: `for` over lists, ranges, and files — `while` with counters and file reading — `until`
- Functions: defining, calling, passing arguments, and returning values
- Script arguments: `$1`–`$9`, `$@`, `$#` — and validating them before use
- Exit codes, `$?`, strict mode with `set -euo pipefail`, and cleanup with `trap`
- Three complete real-world scripts: automated backup, system health check, batch file rename

📂 [Read Chapter 9 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-09-Shell-Scripting)

---

### ✅ **Chapter 10 — Disk Management & the Filesystem in Depth**
How Linux really represents, partitions, formats, and mounts storage — and how to keep it from silently filling up. It covers:
- How Linux names disks and partitions (`/dev/sda`, `/dev/nvme0n1p1`) and the block device model
- Reading disk and partition info with `lsblk` and `fdisk -l`
- Creating partitions interactively with `fdisk` (and when to reach for `parted` instead)
- Formatting partitions with `mkfs.ext4`, `mkfs.xfs`, and other filesystem types
- Mounting and unmounting filesystems with `mount` and `umount`, plus common mount options like `noexec` and `noatime`
- Making mounts persistent and reboot-safe with `/etc/fstab` and UUIDs
- Verifying space and mount status with `df -h`, `df -i`, and `findmnt`
- Logical Volume Management (LVM) basics: `pvcreate`, `vgcreate`, `lvcreate`, and online resizing with `lvextend`
- The real difference between symbolic links and hard links, and how `ln -s` and `ln` behave
- What inodes actually store, and why `stat` and `ls -i` matter when you run out of them with disk space to spare
- Hunting down disk hogs with `du -sh`, and diagnosing `du` vs `df` disagreements
- Creating and managing swap space with `fallocate`, `mkswap`, and `swapon` — including building a swap file from scratch
- Four practical troubleshooting scenarios: new disk setup, "no space left" with free space showing, fixing OOM kills with swap, and mapping what's mounted where

📂 [Read Chapter 10 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-10-Disk-Management-and-Filesystem)

---
### ✅ **Chapter 11 — System Logs, Services & systemd**
Every command you've run so far has been reactive — this is where Linux starts working in the background on its own. It covers:
- Why `systemd` replaced sequential SysVinit scripts, and how PID 1 manages a dependency graph of units
- Units and targets: `.service`, `.timer`, `.mount`, and how targets map to the old runlevels
- Controlling services with `systemctl start`, `stop`, `restart`, `reload`, and `status`
- The real difference between `enable`/`disable` (future boots) and `start`/`stop` (right now), plus `mask`
- Reading logs the modern way with `journalctl`, including `-u`, `-f`, `-e`, and `-r`
- Filtering `journalctl` by `--since`/`--until`, priority level (`-p`), and boot (`-b`)
- The classic `/var/log` files — `syslog`, `auth.log`, `kern.log` — and how they differ by distro
- Keeping logs from growing forever with `logrotate` and its per-app config files
- Writing a complete `systemd` `.service` unit file from scratch, and why `daemon-reload` matters
- Scheduling recurring tasks with `cron`, `crontab -e`, and the five-field time syntax
- Cron shortcuts like `@daily` and `@reboot`, plus system-wide `/etc/cron.d/` and `cron.daily/`
- One-time scheduling with `at`, `atq`, and `atrm`
- Catching up on missed jobs with `anacron` on machines that aren't always powered on
- Four practical scenarios: a service that won't start, a disk filling with logs, setting up a nightly backup, and investigating a boot

📂 [Read Chapter 11 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-11-System-Logs-Services-and-systemd)

---
---

### ✅ **Chapter 12 — What's Next: Linux in the Real World**
The final chapter. You've built the foundation — now here's where it takes you. It covers:

- A complete skill map: every command, concept, and tool covered across all 12 chapters
- Career paths where Linux skills apply directly: sysadmin, DevOps, cybersecurity, cloud, backend, data engineering
- The next layer of tools to learn: `Docker`, `Kubernetes`, `Ansible`, `Terraform`, and Python automation
- Certifications worth pursuing: CompTIA Linux+, LPIC-1/2, RHCSA, RHCE, and CKA — with what each tests
- How to keep learning: `man` pages, the Arch Wiki, official docs, and deliberate practice habits
- Building a home lab: VirtualBox VMs, Raspberry Pi, a cloud VPS, or WSL2 — with project ideas
- The Linux community: Ask Ubuntu, Server Fault, Reddit, Arch Wiki, IRC — and how to ask good questions
- Contributing to open source: documentation, bug reports, and your first pull request
- How this guide was built: the design system, ReportLab, and the philosophy behind the writing

📂 [Read Chapter 12 →](https://github.com/ashihh07/linux-for-beginners/blob/main/Chapter-12-Whats-Next)

---

## Who This Is For

- Complete beginners who have never opened a terminal before
- Windows or macOS users curious about Linux
- Students preparing for tech, cybersecurity, or development careers
- Anyone who wants to understand the systems running behind most servers, cloud platforms, and even their own Android phone

---

## How to Use This Guide

Each chapter builds on the one before it, so it's best to go in order — especially in the early chapters. Open a terminal alongside the guide and actually type the commands as you read. Linux is learned by doing, not just by reading.

---

## A Note on Approach

This guide leans into the terminal early and often, but it doesn't ignore the graphical side of Linux either. You'll get a proper look at desktop environments like GNOME before diving into command-line work, so you understand both faces of the system before choosing which one to lean on.

---

## Contributing

This guide is complete. If you find a typo, an error, or
a command that no longer works on a current Ubuntu release,
please open an Issue and describe the problem.
If you want to suggest an addition or improvement, open
an Issue with your idea before opening a Pull Request.
All contributions are welcome.

---

## License

This project is licensed under the [MIT License](./LICENSE).

---

## Author

**Ashik A** — [github.com/ashihh07](https://github.com/ashihh07)

> This guide was created, organized, refined, and designed using GitHub documentation, industry best practices, publicly available learning resources, and AI-assisted research.

If you find this guide helpful, consider starring the repo ⭐ so others can find it too.
