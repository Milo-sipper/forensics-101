How patch diffing can be used to achieve N-day vulnerabilities
### Fortigate (Firewall)
- prevents attacks and detects unauthorised binaries and prevent them from running 
- Encrypting rootfs.gz using ChaCha20 / XOR
- PIE (Position independent executable)
### Patch diffing
- Used to identify changes between patches to identify potential bugs / exploits
- /bin/init which is a huge monolithic 
- What if we split the /bin/init into logical individual components?
	- Modularity design thinking when building source code even though binary is monolithic
### CVE-2024-231113 - Format string bug in fgfmd
- Allowed an attacker to run code onto a device 
- fgfm protocol:

### CVE-2024-21762 OOB write in sslvpnd
> via malformed HTTPS requests
> 
