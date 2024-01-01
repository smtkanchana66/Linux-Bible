

# Linux Command Bible

<p align="center">
  <img src="https://github.com/smtkanchana66/Linux-Bible/blob/main/res/linux.png" />
</p>



## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Basic Commands](#basic-commands)
4. [File and Directory Management](#file-and-directory-management)
5. [System Administration](#system-administration)
6. [Network Commands](#network-commands)
7. [Package Management](#package-management)
8. [Scripting and Automation](#scripting-and-automation)
9. [Tips and Tricks](#tips-and-tricks)
10. [Contributing](#contributing)
11. [License](#license)

# Introduction

In this section, provide a brief overview of the purpose of the Linux Command Bible and why users should find it valuable.

# Getting Started

If you're new to Linux, start here! This section will cover the basics, including how to access the command line and essential concepts.

# Basic Commands
#### Change Directory
```bash
cd [directory]
```
#### List Files
```bash
ls
```
#### Make Directory
```bash
mkdir [directory_name]
```
#### Create a File
```bash
touch [file_name]
```
#### Copy File
```bash
cp [source_file] [destination]
```
#### Move/Rename File
```bash
mv [old_name] [new_name]
```
#### Remove/Delete File
```bash
rm [file_name]
```
#### Open a File in a Text Editor (e.g., Nano):
```bash
nano [filename]
```
#### Open a File in a Text Editor (e.g., vi):
```bash
vi [filename]
```
<br>

## Git command

#### Clone a Repository from GitHub:
```bash
git clone https://github.com/username/repository.git
```
#### Check Git Status:
```bash
git status
```
#### Stage your changes:
```bash
git add README.md
```
#### Commit the changes:
```bash
git commit -m "Updated Linux Bible in README.md"
``` 
#### Push the changes to GitHub:
```bash
git push origin master
```
> If you're working on a branch other than master, replace it with the appropriate branch name.
> If this is your first time pushing to the repository, Git may prompt you to configure your username and email:
```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
#### Check the status:
```bash
git status
```
<br>

## System Administration

Delve into system administration commands for managing users, processes, and other system-related tasks.

#### Display System Information:
```bash
uname -a
```
#### View CPU Information:
```bash
lscpu
```
#### Check Memory Usage:
```bash
free -m
```
#### Disk Space Usage:
```bash
df -h
```
<br>

## User Management
#### Add a User:
```bash
sudo adduser username
```
#### Add a User to the sudo Group:
```bash
sudo usermod -aG sudo username
```
#### Change User Password:
```bash
passwd username
```
#### Delete a User:
``` bash
sudo deluser username
```
<br>

## System Maintenance

#### Update Package Lists:
```bash
sudo apt update
```
#### Upgrade Installed Packages:
```bash
sudo apt upgrade
```
#### Install a New Package:
```bash
sudo apt install packagename
```
#### Restart the System:
```bash
sudo reboot
```
<br>

## System Logs
#### View System Logs:
```bash
journalctl
```
#### Check Last System Reboot Time:
```bash
last reboot
```
<br>

## Process Management:

#### List Running Processes:
```bash
ps aux
```
#### Kill a Process:
```bash
kill PID
```
#### Check System Load:
```bash
uptime
```

#### Monitor System Resources:
```bash
top
```

<br>

## Network Management:
#### Display Network Configuration:
```bash
ifconfig
```
#### Check Open Ports:
```bash
netstat -tuln
```
#### Verify Connectivity:
```bash
ping example.com
```
#### View Network Statistics:
```bash
netstat -s
```
<br>

## Filesystem Management
#### Check Filesystem Integrity:
```bash
fsck /dev/sda1
```
#### Find Large Files:
```bash
find / -type f -size +100M
```
>Searches for files larger than 100 megabytes on the system.

<br>

## Security:

#### Update Security Packages:
```bash
sudo apt-get install unattended-upgrades
```
```bash
sudo dpkg-reconfigure --priority=low unattended-upgrades
```
>Configures unattended upgrades for automatic security updates.
#### Check for Rootkits:
```bash
rkhunter --check
```
>Scans for rootkits on the system.
#### Firewall Configuration (using UFW):
```bash
sudo ufw status
```
```bash
    sudo ufw allow 22
```
```bash
sudo ufw enable
```
>Checks the firewall status, allows SSH traffic, and enables the firewall.


## System Information:
#### List USB Devices:
```bash
lsusb
```
>Displays information about USB devices connected to the system.

#### Check PCI Devices:
```bash
lspci
```
>Lists PCI devices connected to the system.

### User and Group Management:

30. **List All Users:**
    ```bash
    getent passwd
    ```
    Shows a list of all user accounts on the system.

31. **List All Groups:**
    ```bash
    getent group
    ```
    Displays a list of all groups on the system.

32. **Change User's Primary Group:**
    ```bash
    usermod -g newgroup username
    ```
    Changes the primary group of a user.

### Disk Management:

33. **Check Disk I/O Statistics:**
    ```bash
    iostat
    ```
    Shows disk I/O statistics, including read and write rates.

34. **View Filesystem Mount Points:**
    ```bash
    df -hT
    ```
    Displays information about mounted filesystems, including their type.

### System Performance Monitoring:

35. **Monitor CPU Usage (using `htop`):**
    ```bash
    sudo apt install htop
    htop
    ```
    Interactive process viewer that provides a visual representation of CPU and memory usage.

36. **Check System Temperature (using `lm-sensors`):**
    ```bash
    sudo apt install lm-sensors
    sensors
    ```
    Shows temperature information for various system components.

### Software Package Management:

37. **Search for a Package:**
    ```bash
    apt search packagename
    ```
    Searches for packages related to the specified name.

38. **Remove Unused Dependencies:**
    ```bash
    sudo apt autoremove
    ```
    Removes packages that were installed as dependencies but are no longer needed.

### System Backup and Restore:

39. **Create a System Backup (using `tar`):**
    ```bash
    tar -cvzf backup.tar.gz /path/to/backup
    ```
    Creates a compressed archive of specified files or directories.

40. **Restore from Backup:**
    ```bash
    tar -xvzf backup.tar.gz -C /path/to/restore
    ```
    Extracts files from a compressed archive to the specified restore path.

These commands offer a more comprehensive view of system administration tasks, covering areas such as hardware, user management, disk management, performance monitoring, and more. Always ensure you have a good understanding of the commands and their implications before using them in a production environment. If you have specific tasks or scenarios in mind, feel free to ask for more targeted guidance!

Certainly! Let's delve into some additional system administration commands and tasks for a more comprehensive overview:

### System Maintenance and Updates:

41. **Check for System Updates (using `apt`):**
    ```bash
    sudo apt update
    ```
    Refreshes the package lists to check for available updates.

42. **Clean Package Cache:**
    ```bash
    sudo apt clean
    ```
    Removes downloaded package files from the package cache.

43. **Monitor System Logs (using `journalctl`):**
    ```bash
    journalctl -xe
    ```
    Provides a detailed view of the system logs, aiding in troubleshooting.

### Network Configuration and Troubleshooting:

44. **Configure Network Interfaces:**
    ```bash
    sudo nano /etc/network/interfaces
    ```
    Edit the network configuration file to set up static IP addresses and other network parameters.

45. **DNS Troubleshooting (using `nslookup` or `dig`):**
    ```bash
    nslookup example.com
    ```
    or
    ```bash
    dig example.com
    ```
    Query DNS servers to troubleshoot and verify domain resolution.

### Security and Permissions:

46. **Check File Permissions:**
    ```bash
    ls -l filename
    ```
    Displays detailed file permissions, owners, and groups.

47. **Check System Security Updates (using `unattended-upgrades`):**
    ```bash
    cat /var/log/unattended-upgrades/unattended-upgrades.log
    ```
    Reviews logs for automatic security updates.

### System Monitoring and Resource Usage:

48. **Check System Resource Usage (using `sar`):**
    ```bash
    sudo apt install sysstat
    sar -u
    ```
    Collects, reports, or saves system activity information.

49. **Monitor Disk Space Usage (using `du`):**
    ```bash
    du -h
    ```
    Shows the disk space usage of files and directories in the current location.

### Advanced Process Management:

50. **Monitor Process Resources (using `pidstat`):**
    ```bash
    sudo apt install sysstat
    pidstat 1
    ```
    Monitors resource usage of processes, including CPU, memory, and I/O.

51. **Background Process Management (using `nohup`):**
    ```bash
    nohup command &
    ```
    Runs a command immune to hangups, with output directed to a file.

### Customization and Scripting:

52. **Custom Bash Scripts:**
    Create custom Bash scripts to automate repetitive tasks or perform complex operations.

53. **Configure Shell Environment (using `.bashrc`):**
    Edit the `.bashrc` file to customize the shell environment for users.

These commands cover a broader range of tasks, including network configuration, security, permissions, advanced process management, and customization. Always exercise caution, especially when working with system configurations and sensitive data. If you have specific scenarios or tasks in mind, feel free to ask for more detailed guidance!
-->

## Network Commands

Discover commands for network configuration, troubleshooting, and other networking essentials.

## Package Management

Explore package management commands for installing, updating, and removing software packages.

## Scripting and Automation

Get into the world of scripting and automation with examples and explanations of scripting languages commonly used in Linux.

## Tips and Tricks

This section will provide various tips and tricks to enhance your Linux command-line experience.

## Contributing

We welcome contributions! If you have additional commands, examples, or improvements, please follow our contribution guidelines.

## License

This Linux Command Bible is licensed under [License Name]. See the [LICENSE](LICENSE) file for details.

