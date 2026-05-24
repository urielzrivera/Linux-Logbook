# Nmap

Initial Scan
```bash
nmap -sV -sC $IP -oN recon/initial
```

Scan all ports
```bash
nmap -sV -sC -T4 -v -p- $IP -oN recon/all_ports
```

UDP Scan
```bash
nmap -sU -sV -sC -n -F -T4 $IP -oN recon/udp_scan
```

# Webservers

Directory Discovery
```bash
gobuster dir -w /path/to/wordlist -u $IP
```

Virtual Host Discovery
```bash
gobuster vhost -u https://example.com -w /path/to/wordlist
```
