# Pentesting-Notes

hi there, 

Welcome to my Pentesting Notebook.\
This serves as a living document for every useful command, tactics, techniques, and procedures learned during pentesting engagements, labs, CTFs, or interacting with the security community.

## VM Setup and Post-Installation Tasks

#### Verifying Checksums
##### Windows
```bash
certutil -hashfile \path\to\file <algorithm>
```

##### Linux / OS X / Unix
```bash
shasum -a algorithm /path/to/file/
```
---

### Post-Installation Tasks [Securing Linux]

Change default credentials
```bash
passwd
```
Create standard user
```bash
sudo adduser username
```
Create standard user with zsh [Kali]
```bash
sudo useradd -m -s /usr/bin/zsh newuser
```

Grant sudo permissions
```bash
sudo usermod -aG sudo username
```

Apply Kali Visual theme
```bash
sudo cp /etc/skel/.zshrc /home/newuser/
sudo chown newuser:newuser /home/newuser/.zshrc
```

Verify shell
```bash
sudo chsh -s /bin/bash username
```

Verify user directory creation
```bash
ls /home
```

Check for extra users
```bash
cat /etc/passwd
```
## Maintenance 
```bash
sudo apt update && sudo apt full-upgrade -y
```

## Useful Commands
Set target IP variable
```bash
export IP=target_ip
```
```bash
echo $IP
```

## Tools

Checking for installed tools

Check if the system can locate the tool's executable binary
```bash
which tool_name
```

Check for tool in Kali's repositories
```bash
apt list tool_name
```

