hi there,

welcome to my pentesting notebook.

this repository serves as a living KB that documents useful commands, methodologies, tactics, techniques, and procedures i've learned throughout my journey in offensive security. the content here is continuously updated as i gain experience through penetration testing labs, CTF challenges, research, community knowledge, and real-world engagements.

the *goal* of this notebook is to consolidate information that i find valuable enough to revisit regularly, and spend less time searching for commands, techniques, and workflows.

### A Living Document

security is constantly evolving, and so is this repository.
if you find anything here useful, that's a bonus. 

happy hacking, and happy learning.

## VM Setup and Post-Installation Tasks

# What You'll Find Here

this repository contains notes and references for topics such as:

* Notetaking
* Reconnaissance and enumeration
* Web application testing
* Active Directory assessments
* Privilege escalation
* Credential attacks
* Exploitation techniques
* Post-exploitation activities
* Reporting and documentation
* Tool usage and common command references and cheat sheets

# README Contents

this README includes many of the commands, setup procedures, tools, and quick-reference notes that i commonly use when:
* configuring Kali Linux virtual machines
* preparing for labs or CTFs
* building new testing environments
* conducting live assessments
* troubleshooting tooling issues
* documenting findings and evidence

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
## Notetaking
### vim
Useful vim commands

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
### Tool Library
