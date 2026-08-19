# Laboratory 01 – Welcome to the Cloud

## Mission Overview

This laboratory activity is the first step in learning cloud computing and cloud infrastructure. We used the KillerCoda Ubuntu Playground to practice working in a Linux environment and created a GitHub repository to serve as our Cloud Computing Portfolio. The activities helped us become familiar with basic Linux commands, system information, file management, Markdown documentation, and GitHub.

## Objectives

* Access and use a Linux environment through KillerCoda.
* Create and manage a Linux user account.
* Explore the Linux operating system and gather system information.
* Create and organize files and directories using Linux commands.
* Create and maintain a public GitHub repository.
* Practice documenting technical activities using Markdown.

## Activities Performed

During the laboratory activity, we launched an Ubuntu 24.04 environment using KillerCoda and verified that the terminal was working properly. We created a new Linux user named pfonacier, assigned a password, provided sudo privileges, and logged in using the new account. We also gathered information about the Linux distribution, kernel version, CPU, memory, and available disk space. We created folders and a Markdown file for our workspace and prepared a GitHub repository named CCM101-smtejano to organize our laboratory outputs. Screenshots and documentation were also prepared as part of our Cloud Computing Portfolio.

## Linux Commands Used

The following Linux commands were used during the laboratory activity:

```bash
whoami
pwd
hostname
useradd -m -s /bin/bash pfonacier
passwd pfonacier
usermod -aG sudo pfonacier
su - pfonacier
cat /etc/os-release
uname -r
lscpu | grep "Model name"
free -h
df -h /
mkdir Documents Notes Reports Screenshots
ls
cd  Notes
pwd
nano about-me.md
cat about-me.md

## Skills Learned

Through this laboratory activity, I learned how to access and work with a Linux environment using KillerCoda. I learned how to create and manage a Linux user account and use basic Linux commands to navigate and manage files and directories. I also learned how to check important system information such as the operating system, kernel, CPU, memory, and disk space. In addition, I gained experience in creating a GitHub repository and organizing technical documentation using Markdown. Overall, this activity helped me develop basic Linux, documentation, and GitHub skills that will be useful for future cloud computing activities.
