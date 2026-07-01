# Day 2 - Linux File System

## 📖 What is the Linux File System?

The Linux file system is a hierarchical structure that organizes all files and directories under a 
single root directory (`/`). Unlike Windows, Linux does not use drive letters such as `C:` or `D:`.

---

# Linux Directory Structure

```
/
├── bin
├── boot
├── dev
├── etc
├── home
├── lib
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── srv
├── sys
├── tmp
├── usr
└── var
```

---

# Important Directories

## `/`
The root directory. Every file and directory starts from here.

---

## `/home`

Stores personal files of users.

Example:

```
/home/shoaib
```

---

## `/root`

Home directory of the root (administrator) user.

---

## `/bin`

Contains essential user commands.

Examples:

```
ls
cp
mv
cat
pwd
```

---

## `/sbin`

Contains system administration commands.

Examples:

```
shutdown
reboot
fdisk
```

---

## `/etc`

Stores system configuration files.

Examples:

```
passwd
hosts
ssh
fstab
```

---

## `/var`

Contains variable data such as:

- Logs
- Mail
- Cache
- Databases

Example:

```
/var/log/syslog
```

---

## `/tmp`

Stores temporary files.

Usually cleaned automatically after reboot.

---

## `/usr`

Contains installed applications and utilities.

Examples:

```
/usr/bin
/usr/lib
/usr/share
```

---

## `/boot`

Contains files required to boot Linux.

Examples:

- Linux Kernel
- GRUB Bootloader

---

## `/dev`

Contains device files.

Examples:

```
/dev/sda
/dev/null
/dev/tty
```

---

## `/proc`

A virtual filesystem containing process and kernel information.

Useful commands:

```bash
cat /proc/cpuinfo
cat /proc/meminfo
```

---

## `/sys`

Contains information about hardware and kernel devices.

---

## `/media`

Used for automatically mounted devices.

Example:

```
USB Drive
DVD
```

---

## `/mnt`

Used for manually mounting storage devices.

---

## `/opt`

Stores optional third-party software.

---

# Useful Commands

### Print Current Directory

```bash
pwd
```

---

### List Files

```bash
ls
```

---

### Long Listing

```bash
ls -l
```

---

### Show Hidden Files

```bash
ls -la
```

---

### Change Directory

```bash
cd /home
```

---

### Go to Previous Directory

```bash
cd ..
```

---

### Go to Home Directory

```bash
cd ~
```

---

### Display Directory Tree

```bash
tree
```

> Install if needed:

```bash
sudo apt install tree
```

---

# Practice Exercises

1. Display the current directory.
2. Navigate to `/etc`.
3. List all files, including hidden files.
4. Move to your home directory.
5. Explore the `/var/log` directory.
6. View CPU information using `/proc/cpuinfo`.
7. Install and use the `tree` command.

---

# Interview Questions

### 1. What is the Linux file system?

A hierarchical structure that organizes files and directories under the root (`/`) directory.

---

### 2. What is the difference between `/home` and `/root`?

- `/home` stores regular users' home directories.
- `/root` is the home directory of the root user.

---

### 3. What is stored inside `/etc`?

System-wide configuration files.

---

### 4. What is `/proc`?

A virtual filesystem that provides information about running processes and the Linux kernel.

---

### 5. Why is `/tmp` used?

It stores temporary files created by applications and the operating system.

---

# Summary

- Linux uses a hierarchical file system.
- Everything begins from the root directory (`/`).
- Configuration files are in `/etc`.
- User data is in `/home`.
- Logs are stored in `/var/log`.
- Devices are represented in `/dev`.
- Process information is available in `/proc`.
