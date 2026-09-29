# Linux System Information and Resource Monitoring Tool

A C-based Linux terminal application for monitoring system resources and displaying important system information through a simple menu-driven interface.

## Overview

The Linux System Information and Resource Monitoring Tool provides a centralized way to monitor essential Linux system resources such as CPU, memory, disk storage, processes, network activity, and system uptime.

The application is developed in C and uses Linux system interfaces, system calls, and the `/proc` filesystem to collect and process system information directly from the operating system.

This project was developed to demonstrate practical Operating System concepts including process management, memory management, file system management, CPU utilization, system calls, and resource management.

## Features

- **System Information**
  - Operating system and kernel information
  - System architecture
  - Hostname
  - CPU information
  - CPU cores and frequency
  - Current user information

- **CPU Usage Monitoring**
  - CPU utilization percentage
  - Continuous CPU monitoring
  - CPU statistics using `/proc/stat`

- **Memory Monitoring**
  - Total, used, and available RAM
  - Cached and buffer memory
  - Swap memory usage
  - Memory utilization status

- **Disk Monitoring**
  - Total, used, and free disk space
  - Disk utilization percentage
  - Inode statistics

- **Process Monitoring**
  - Running processes
  - Process ID (PID)
  - Parent Process ID (PPID)
  - Process states
  - Process hierarchy

- **System Uptime**
  - Days, hours, minutes, and seconds
  - Total system uptime
  - Cumulative CPU time

- **System Health Summary**
  - CPU usage status
  - Memory usage status
  - Disk usage status
  - Process activity overview

- **Network Monitoring**
  - Network interfaces
  - Received data
  - Transmitted data
  - Network activity

- **Top Resource-Consuming Processes**
  - Top CPU-consuming processes
  - Top memory-consuming processes
  - Process resource statistics

- **Process Search**
  - Search processes by PID
  - Search processes by name

- **Resource Alerts**
  - CPU usage threshold monitoring
  - Memory usage threshold monitoring
  - Disk usage threshold monitoring

- **Resource Usage Logging**
  - Timestamped resource information
  - CPU, memory, disk, and process statistics
  - Log storage in `monitor_log.txt`

## Technologies Used

- C Programming
- Linux / Ubuntu
- GCC Compiler
- Linux Terminal
- Visual Studio Code
- `/proc` Filesystem
- Linux System Calls
- POSIX APIs

## Linux Interfaces Used

The project uses Linux system interfaces to obtain live system information:

```text
/proc/cpuinfo
/proc/stat
/proc/meminfo
/proc/uptime
/proc/net/dev
/proc/[PID]/stat
/proc/[PID]/statm
