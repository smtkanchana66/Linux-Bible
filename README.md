

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

## Getting Started

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
# Git command

#### Clone a Repository from GitHub:
```bash
git clone https://github.com/username/repository.git
```
### Check Git Status:
```bash
git status
```
### Stage your changes:
```bash
git add README.md
```
### Commit the changes:
```bash
git commit -m "Updated Linux Bible in README.md"
``` 
### Push the changes to GitHub:
```bash
git push origin master
```
> If you're working on a branch other than master, replace it with the appropriate branch name.
> If this is your first time pushing to the repository, Git may prompt you to configure your username and email:
```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
### Check the status:
```bash
git status
```

# System Administration

Delve into system administration commands for managing users, processes, and other system-related tasks.

### Display System Information:
```bash
uname -a
```
### View CPU Information:
```bash
lscpu
```
### Check Memory Usage:
```bash
free -m
```
### Disk Space Usage:
```bash
df -h
```
## User Management
### Add a User:
```bash
sudo adduser username
```
### Add a User to the sudo Group:
```bash
sudo usermod -aG sudo username
```
### Change User Password:
```bash
passwd username
```
### Delete a User:
``` bash
sudo deluser username
```
## System Maintenance
### Update Package Lists:
```bash
sudo apt update
```
### Upgrade Installed Packages:
```bash
sudo apt upgrade
```
### Install a New Package:
```bash
sudo apt install packagename
```
### Restart the System:
```bash
sudo reboot
```
## System Logs
### View System Logs:
```bash
journalctl
```
### Check Last System Reboot Time:
```bash
last reboot
```

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

