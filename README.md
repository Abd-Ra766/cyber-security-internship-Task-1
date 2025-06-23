# Cyber Security Internship - Task 1: Port Scanning

## ✅ Objective
To perform a TCP SYN scan on my local network to discover open ports and understand network exposure.

## 🛠 Tools Used
- Nmap
- Windows Command Prompt

## 🧪 Steps Followed
1. Installed Nmap from the official website.
2. Found my local IP range: 192.168.1.0/24
3. Ran the command: `nmap -sS 192.168.1.0/24`
4. Saved the output as `scan_results.txt`

## 🔍 Sample Output Summary
### 192.168.1.1
- Port 80 (HTTP): Open
- Port 443 (HTTPS): Open

### 192.168.1.10
- Port 22 (SSH): Open
- Port 8080 (HTTP-Proxy): Open

### 192.168.1.15
- Port 139 (NetBIOS-SSN): Open
- Port 445 (Microsoft-DS): Open

## ⚠️ Security Analysis
- Open SSH port (22) can be risky if password authentication is enabled.
- Port 8080 can be vulnerable to proxy attacks if not secured.
- SMB ports (139, 445) are often targeted for ransomware attacks.

## 📎 File List
- `scan_results.txt` - Nmap scan result
- `README.md` - This documentation

## 📝 Conclusion
This task helped me understand how devices on a network expose services through open ports and how these can pose potential security risks.
