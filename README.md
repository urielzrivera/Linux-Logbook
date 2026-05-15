# Pentesting-Notes

## Lab Setup

#### Verifying Checksums
##### Windows
```bash
certutil -hashfile \path\to\file <algorithm>
```

##### Mac/Unix
```bash
shasum -a <algorithm> /path/to/file/
```

#### Kali Linux Post-Install

Change default credentials
```bash
passwd
```

Check for extra users
```bash
cat /etc/passwd
```
