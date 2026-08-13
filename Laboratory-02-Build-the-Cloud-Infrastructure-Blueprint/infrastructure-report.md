# Infrastructure Report

## Linux Server Investigation

The Linux server was investigated using the KillerCoda terminal.

| Information | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel Version | 6.8.0-136-generic |
| CPU Model | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU Cores | 1 |
| Total RAM | 1.9 GiB |
| Disk Capacity | 19 GB |
| Mounted File Systems | /run, /, /dev/shm, /run/lock, /boot, /boot/efi |
| Hostname | ubuntu |
| IP Address | 172.30.1.2, 172.17.0.1 |

## Commands Used

- `cat /etc/os-release` - checked the operating system.
- `uname -r` - checked the kernel version.
- `lscpu` - checked the CPU information.
- `nproc` - checked the number of CPU cores.
- `free -h` - checked the RAM.
- `df -h` - checked the disk capacity and mounted file systems.
- `hostname` - checked the hostname.
- `hostname -I` - checked the IP addresses.

## Observation

The KillerCoda Linux server is running Ubuntu 24.04.4 LTS. It has one CPU core, 1.9 GiB of RAM, and a 19 GB main disk. The server also has several mounted file systems and two IP addresses.
