# Changelog

All important improvements, new features, and fixes are described below.

---

## [1.1.0] - 2026-05-03

### 🆕 New Features

#### 🇬🇧 English Language
- Added complete localization to English. Switch between SK and EN anytime while using the software.

#### 🔗 Timeline of network connections
- New timeline view shows **when a network connection first appeared** and when it disappeared. Great for tracking suspicious activity over time.

#### 📊 New charts
- **RX/TX traffic chart** for each selected connection – see real-time data sent and received.
- **Top 5 processes chart** – which programs consume the most network bandwidth.

#### 🔍 One-click connection details
- One-click connection details now include:
  - WHOIS / RDAP – who owns the remote server
  - Ping – connection response time
  - Traceroute – packet path through the internet
  - DNS / reverse DNS – domain name for an IP address
  - TLS certificate – security certificate of the remote server

#### 🧠 Process forensics
- Enhanced process forensics:
  - List of loaded libraries (DLLs)
  - SHA-256 hash – unique digital fingerprint
  - File size, version, metadata
  - Process tree – parent-child relationships

#### 🔎 Memory string search
- Scan memory of any process for readable text strings (ASCII / Unicode). Useful for finding hidden commands or URLs.

#### 🛡️ Reputation and threat-intel panels
- Reputation and threat intelligence panels:
  - VirusTotal – IP reputation check
  - Hybrid Analysis – file analysis by SHA-256
  - GreyNoise – detect if IP is a security scanner or attacker
  - Dedicated **alerts table** – all suspicious findings in one place

#### 🛡️ Anti-BSOD protection
- When attempting to kill a process, the software **assesses the risk**. Dangerous system processes are blocked or require confirmation. No more Blue Screen of Death.

#### ☁️ Improved cloud services handling
- API responses are now **cached** – faster loading, fewer API calls consumed.
- Better **retry and timeout logic** – graceful handling when services are slow.

#### 🔐 API key security
- Your API keys (e.g., for VirusTotal) are now stored **encrypted**, not as plain text. Your keys stay safe.

---

### 🔧 Fixes & Improvements

#### 🧹 Better IP filtering
- Better IP filtering:
  - Fixed IPv6 and IPv4-mapped address normalization
  - Now correctly ignores:
    - Private IPs (192.168.x.x, 10.x.x.x, 172.16.x.x)
    - CGNAT addresses (100.64.x.x)
    - Multicast, documentation, and reserved ranges

#### 🚪 Clean application shutdown
- Clean application shutdown – all timers, background tasks, and connections are properly stopped.

#### 🔄 Update checker
- Update checker now reads your **actual software version**. No more false "new version 1.0.0" notifications.

#### 🌐 Translation system
- Most dialog windows and messages are now translated. Less English when using Slovak language.

---

## [1.0.0] - 2026-04-15

### 🎉 Initial release
- First public release of SW-NET Forensic

---

*Last updated: 2026-05-03*
