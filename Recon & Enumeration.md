# Nmap

Initial Scan
```bash
nmap -sV -sC $IP -oN nmap/initial
```

Scan all ports
```bash
nmap -sV -sC -T4 -v -p- $IP -oN nmap/all_ports
```

UDP Scan
```bash
nmap -sU -sV -sC -n -F -T4 $IP -oN nmap/udp_scan
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
