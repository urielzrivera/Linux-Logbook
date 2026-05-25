# Webservers

Directory Discovery
```bash
gobuster dir -w /path/to/wordlist -u $IP
```

Virtual Host Discovery
```bash
gobuster vhost -u https://example.com -w /path/to/wordlist
```
Adding primary domains to `/etc/hosts`

```bash
echo "$IP domain.name" | sudo tee -a /etc/hosts
```
* Use when failing to resolve a site
* Overrides DNS resolution, forcing your machine to map specific domain names to target IPs
