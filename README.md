<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Share+Tech+Mono&weight=700&size=28&pause=1000&color=CC0000&center=true&vCenter=true&width=700&lines=Anas+Labrini;Independent+Security+Researcher;Red+Team+Practitioner;Offensive+Tool+Developer" alt="Typing SVG" />

</div>

---

## Identity

**Anas Labrini** is an independent cybersecurity researcher and Red Team practitioner based in Morocco, specializing in offensive security operations, adversary simulation, and the development of research-grade security tooling for authorized testing environments.

His trajectory began through rigorous self-directed study across Linux systems internals, network architecture, and Python-based automation, before progressing into penetration testing methodology, exploit development, and post-exploitation engineering. He has completed structured hands-on training under the supervision of experienced practitioners in the field.

His work centers on translating theoretical attack knowledge into functional tooling — spanning reconnaissance automation, payload delivery mechanisms, command and control infrastructure, anti-forensics research, and post-assessment analysis — operating exclusively within legally authorized and ethical boundaries.

---

## Disciplines

Reconnaissance — Passive and Active  
Initial Access and Exploitation  
Privilege Escalation  
Lateral Movement and Pivoting  
Post-Exploitation Engineering  
Persistence Mechanisms  
Defense Evasion and Anti-Forensics  
Command and Control Infrastructure  
Web Application Security Testing  
Network Attack Simulation  
Social Engineering and Phishing Simulation  
Credential Access and Exfiltration Research  
Adversary Simulation and Threat Emulation  
OSINT and Intelligence Gathering  

---

## Technical Stack

**Operating Systems:** Linux — Primary offensive platform  
**Languages:** Python, PowerShell, Bash, C (DigiSpark), VBScript  
**Frameworks and C2:** Metasploit, Cobalt Strike, Empire, Sliver  
**Network and Reconnaissance:** Nmap, Masscan, Wireshark, Tcpdump, Bettercap  
**Web Application:** Burp Suite, SQLmap, Ffuf, Gobuster, Feroxbuster  
**Credential Attacks:** Hashcat, John the Ripper, Hydra, Medusa, Responder  
**Active Directory:** BloodHound, SharpHound, Evil-WinRM, Impacket  
**Enumeration:** LinPEAS, WinPEAS  
**OSINT:** TheHarvester, Amass  

---

## Developed Tools

The following tools were designed, engineered, and maintained by Anas Labrini as part of his independent security research. Each project reflects a specific domain of offensive operations and serves as both a functional testing instrument and a research artifact.

---

### CROSSMOS
**Category:** Red Team / Adversary Simulation / Malware Research  
**Language:** C (DigiSpark), PowerShell, Python  
**Platform:** Windows  

A USB-deployable, modular Red Team attack framework built around a full Windows operational architecture. CROSSMOS implements a multi-component design with clearly separated functional roles across installation, command and control, payload execution, activity monitoring, anti-AV awareness, tamper detection, and secure self-destruction.

The command and control engine leverages the Telegram Bot API over HTTPS for low-noise, bidirectional communication — a living-off-the-land approach that avoids traditional C2 infrastructure signatures. The framework incorporates advanced persistence through scheduled tasks with SYSTEM-level privileges, defense evasion via PowerShell logging suppression and timestomping, credential extraction from Chromium-based browsers using DPAPI and AES-GCM decryption, keylogging with foreground window correlation, GPS and network reconnaissance, and a layered self-destruction protocol that eliminates filesystem artifacts, shadow copies, event logs, prefetch data, and USN journal records.

An anti-VM and sandbox detection engine uses hardware fingerprinting, ACPI inspection, MAC address OUI profiling, timing analysis, and system age heuristics to evaluate the execution environment prior to payload activation. Payload protection is implemented through a triple AES-256 encryption pipeline with code obfuscation and Python-to-C transpilation into compiled .pyd modules.

MITRE ATT&CK coverage includes: T1555, T1040, T1059, T1105, T1564, T1057, T1113, T1562, T1071, T1027, T1082, T1518, T1083, T1056.

Repository: [github.com/anaslabrini/crossmos](https://github.com/anaslabrini/crossmos)

---

### SpyMorph
**Category:** Offensive Security / Red Team Research  
**Platform:** Linux — Root-level execution  

A multi-stage, multi-layered offensive security framework demonstrating advanced Red Team techniques including execution flow control, payload concealment, staged decryption, stealth execution, in-memory code execution, and long-term systemd-based persistence.

The execution chain is designed as a sequence of isolated stages: an entry dispatcher, a decryption loader, an encrypted data container, a stealth execution and cleanup layer, and a remotely hosted encrypted persistence payload. Each stage is minimal and terminates silently on failure, producing no recoverable artifacts. The persistence layer operates through systemd service files, restores automatically if stopped, and runs with near-zero system resource consumption. The framework includes anti-forensics capabilities through in-memory execution via exec(), file overwriting with random data, and secure self-deletion of critical components.

Repository: [github.com/anaslabrini/SpyMorph](https://github.com/anaslabrini/SpyMorph)

---

### S-PUP (Shark Pup)
**Category:** Surveillance Research / Persistence Engineering / Credential Access  
**Platform:** Cross-platform — Windows, Linux, macOS  

An advanced cross-platform surveillance and persistence research tool combining keylogging, system reconnaissance, credential extraction, anti-analysis evasion, and a resilient multi-layered persistence architecture.

On execution, S-PUP establishes five independent persistence paths across hidden directories, each functioning as a guardian process that monitors the primary agent. If the main instance is terminated or removed, any surviving guardian restores the full operational state within a 60-minute cycle. The system also performs automatic self-updates from a remote repository at the same interval, enabling deployment of post-exploitation expansions without re-access to the target.

Reconnaissance capabilities include: OS and hardware enumeration, internal and external IP addresses, MAC address resolution, Wi-Fi network profiles, active processes, installed applications, file listings from Desktop, Downloads, and Documents, open TCP/UDP connections, network-adjacent device discovery, and extraction of stored credentials from Chrome and Firefox. Keystrokes are logged in sessions of 50 keystrokes and delivered via email or Telegram. Anti-analysis features scan for and disable known forensic, reverse engineering, and analysis tools including Wireshark, Process Hacker, IDA Pro, Ghidra, GDB, and Frida.

The delivery component is a VBScript dropper that silently generates and executes a PowerShell loader, detects system architecture, deploys a portable embedded Python 3.11 environment, installs required libraries, fetches the payload from a remote source, launches it, and removes all loader artifacts — operating without visible user interaction or security alerts.

Persistence mechanisms by platform: systemd user services on Linux, Startup folder batch files on Windows, LaunchAgent plist entries on macOS.

Repository: [github.com/anaslabrini/S-PUP](https://github.com/anaslabrini/S-PUP)

---

### AnasC2
**Category:** Command and Control / Browser-Based Agent Control  
**Language:** Python — Flask, Socket.IO  

A browser-based Command and Control framework providing real-time bidirectional control over agent sessions via WebSocket communication. The admin panel enables operators to redirect connected agents to arbitrary URLs and deliver alert payloads. Additional modules include an HTTP status code checker and a directory scanner driven by a custom wordlist. All modules are accessible through a centralized launcher interface.

Repository: [github.com/anaslabrini/AnasC2](https://github.com/anaslabrini/AnasC2)

---

### AnasHunter
**Category:** Web Application Security Testing  
**Language:** Python  

A modular web application penetration testing framework covering cross-site scripting detection, SQL injection scanning, clickjacking vulnerability identification, brute force attack execution, and denial-of-service testing. Each attack vector is isolated in a dedicated module and invoked through a unified launcher.

Repository: [github.com/anaslabrini/AnasHunter](https://github.com/anaslabrini/AnasHunter)

---

### AnasOsint
**Category:** Open Source Intelligence / Reconnaissance Automation  
**Language:** Python  

A modular OSINT intelligence framework supporting structured reconnaissance across email addresses, phone numbers, IP addresses, and domains. Each lookup module operates in basic and advanced modes, aggregating data from over 20 external sources per target type. Sources include HaveIBeenPwned, Hunter.io, Shodan, Censys, AbuseIPDB, VirusTotal, GreyNoise, SecurityTrails, crt.sh, WHOIS, DNS record analysis, and others. Results can be saved as timestamped reports. Both interactive menu and command-line execution modes are supported.

Repository: [github.com/anaslabrini/AnasOsint](https://github.com/anaslabrini/AnasOsint)

---

### AnasRecon
**Category:** Website Reconnaissance / Asset Discovery  
**Language:** Python  

A deep reconnaissance framework for web targets providing: domain and IP resolution, WHOIS lookup, ASN and IPInfo data, subdomain enumeration, SSL certificate inspection, HTTP security header analysis, sensitive keyword detection in page content, Nmap-based port and service enumeration, web vulnerability checks for XSS, SQL injection, and CSRF, Shodan host integration, and a final risk scoring assessment across High, Medium, and Low severity categories. All results are written to structured text reports.

Repository: [github.com/anaslabrini/AnasRecon](https://github.com/anaslabrini/AnasRecon)

---

### AnassRedTool
**Category:** Multi-Function Red Team Toolkit  
**Language:** Python  

A multi-purpose offensive toolkit covering SSH, FTP, and HTTP brute-force attacks with custom wordlist support, port scanning for open service identification, and host availability testing. Designed for streamlined Red Team workflow integration.

Repository: [github.com/anaslabrini/AnassRedTool](https://github.com/anaslabrini/AnassRedTool)

---

### AnaSSHoney
**Category:** Honeypot / Threat Intelligence  

A high-interaction SSH honeypot system for capturing attacker behavior, credential attempts, and session activity in controlled environments.

Repository: [github.com/anaslabrini/AnasSSHoney](https://github.com/anaslabrini/AnasSSHoney)

---

## GitHub Statistics

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=anaslabrini&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&title_color=CC0000&icon_color=CC0000&text_color=FFFFFF" width="48%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=anaslabrini&layout=compact&theme=radical&hide_border=true&bg_color=0D1117&title_color=CC0000&text_color=FFFFFF" width="48%" />

</div>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=anaslabrini&theme=radical&hide_border=true&background=0D1117&ring=CC0000&fire=CC0000&currStreakLabel=CC0000" width="65%">

</div>

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=anaslabrini&custom_title=Contribution+Graph&bg_color=0D1117&color=CC0000&line=CC0000&point=FFFFFF&area_color=0D1117&hide_border=true" width="98%"/>

</div>

---

## Contact

All documented projects and technical work are publicly available at [github.com/anaslabrini](https://github.com/anaslabrini).

For professional inquiries, training verification, or access to sanitized assessment reports, contact can be made through the official email address listed on the website: [anaslabrini.netlify.app](https://anaslabrini.netlify.app)

---

<div align="center">

All tools and projects documented in this profile are developed exclusively for educational purposes, authorized penetration testing, Red Team simulation, and security research. Unauthorized use against systems without explicit written permission is illegal. The author assumes no responsibility for misuse.

![Profile Views](https://komarev.com/ghpvc/?username=anaslabrini&color=CC0000&style=flat-square&label=Profile+Views)

</div>
