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

##### Mac/Unix
```bash
shasum -a <algorithm> /path/to/file/
```
---

### Post-Installation Tasks [Securing Kali Linux]

Change default credentials
```bash
passwd
```

Check for extra users
```bash
cat /etc/passwd
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

