

# Linux Command Bible

<p align="center">
  <img src="https://github.com/smtkanchana66/Linux-Bible/blob/main/res/linux.png" />
</p>



# Table of Contents

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




# Git command

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
> [!IMPORTANT]
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




# System Administration

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



# User Management 

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



# System Maintenance

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




# System Logs

#### View System Logs:
```bash
journalctl
```
#### Check Last System Reboot Time:
```bash
last reboot
```
<br>



# Process Management

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




# Network Management

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



# Filesystem Management

#### Check Filesystem Integrity:
```bash
fsck /dev/sda1
```
#### Find Large Files:
```bash
find / -type f -size +100M
```
> [!NOTE]
>Searches for files larger than 100 megabytes on the system.
<br>




# Security

#### Update Security Packages:
```bash
sudo apt-get install unattended-upgrades
```
```bash
sudo dpkg-reconfigure --priority=low unattended-upgrades
```
#### Check for Rootkits:
```bash
rkhunter --check
```
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
> [!NOTE]
>Checks the firewall status, allows SSH traffic, and enables the firewall.
<br>


# System Information

#### List USB Devices:
```bash
lsusb
```
#### Check PCI Devices:
```bash
lspci
```
> [!NOTE]
>Lists PCI devices connected to the system.
<br>

# User and Group Management

#### List All Users:
```bash
getent passwd
```
> [!NOTE]
>Shows a list of all user accounts on the system.

#### List All Groups:
```bash
getent group
```
#### Change User's Primary Group:
```bash
usermod -g newgroup username
```
<br>



# Disk Management

#### Check Disk I/O Statistics:
```bash
iostat
```
#### View Filesystem Mount Points:**
```bash
df -hT
```
<br>



# System Performance Monitoring

#### Monitor CPU Usage (using `htop`)
```bash
sudo apt install htop
htop
```
> [!NOTE]
>Interactive process viewer that provides a visual representation of CPU and memory usage.

#### Check System Temperature (using `lm-sensors`)
```bash
sudo apt install lm-sensors
sensors
```
<br>



# Software Package Management

#### Search for a Package:
```bash
apt search packagename
```
#### Remove Unused Dependencies:
```bash
sudo apt autoremove
```
<br>



# System Backup and Restore

#### Create a System Backup (using `tar`):
 ```bash
 tar -cvzf backup.tar.gz /path/to/backup
 ```

#### Restore from Backup:
```bash
tar -xvzf backup.tar.gz -C /path/to/restore
```
<br>


# System Maintenance and Updates

#### Check for System Updates (using `apt`):
```bash
sudo apt update
```

### Clean Package Cache:
```bash
sudo apt clean
```
### Monitor System Logs (using `journalctl`):
```bash
journalctl -xe
```
<br>
    
# Network Configuration and Troubleshooting:

#### Configure Network Interfaces:
```bash
sudo nano /etc/network/interfaces
```
#### DNS Troubleshooting (using `nslookup` or `dig`):
```bash
nslookup example.com
```
or
```bash
dig example.com
```
<br>



# Security and Permissions

#### Check File Permissions:
```bash
ls -l filename
```

#### Check System Security Updates (using `unattended-upgrades`):
```bash
cat /var/log/unattended-upgrades/unattended-upgrades.log
```
<br>


# System Monitoring and Resource Usage:

#### Check System Resource Usage (using `sar`):
```bash
sudo apt install sysstat
sar -u
```
#### Monitor Disk Space Usage (using `du`):
```bash
du -h
```
<br>

# Advanced Process Management

#### Monitor Process Resources (using `pidstat`):
```bash
sudo apt install sysstat
pidstat 1
```

# Background Process Management (using `nohup`):
```bash
nohup command &
```
<br>


# License

This Linux Command Bible is licensed under [Apache-2.0 license]. See the [LICENSE](LICENSE) file for details.


