

## 📋 Project Overview

This project documents the process of identifying, analyzing, and mitigating security vulnerabilities discovered during a Nessus scan

## 🛠 Tools Used

- **Nessus Essentials** – Vulnerability scanning

---

## 🔍 Step-by-Step Process

### 1. ⚙️ Vulnerability Scanning
- Performed a scan using **Nessus Essentials**
- Host scanned: `192.168.1.47`

### 2. 🧠 Vulnerability Analysis
Each vulnerability was interpreted manually using CVE information and plugin data from Nessus:

| Vulnerability | Severity | Description |
|---------------|----------|-------------|
| Node.js < 18.19.1 / 20.x < 20.11.1 / 21.x < 21.6.2 | Critical | Multiple flaws including HTTP/2 DoS, environment variable handling |
| Node.js < 18.20.1 / 20.12.1 / 21.7.2 | High | HTTP/2 race condition and request smuggling |
| Node.js < 18.20.4 / 20.15.1 / 22.4.1 | High | RCE via child_process and permission bypass |
| Node.js < 18.20.6 / 20.18.2 / 22.13.1 / 23.6.1 | High | Worker thread leaks and memory issues |
| Node.js < 20.19.2 / 22.15.1 / 23.11.1 / 24.0.2 | Medium | Unsafe cryptographic operations |
| Python Tornado < 6.5.0 | High | DoS via malformed multi-part data |
| SSL Certificate Cannot Be Trusted | Medium | Self-signed/expired certs |

### 3. ✅ Mitigation
For each finding, mitigation steps were provided. These included:

- Upgrading affected packages (Node.js, Tornado)
- Disabling risky features (e.g., HTTP/2 where not needed)
- Hardening systems (e.g., permissions, proxies)
- Replacing untrusted SSL certificates

