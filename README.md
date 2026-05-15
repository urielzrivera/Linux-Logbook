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

#### Post-Install

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
export IP=<target ip>
```
```bash
echo $IP
```
