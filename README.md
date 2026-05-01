<div align="center">

<h1 style="letter-spacing:1px;">ANAS LABRINI</h1>
<p><strong>Offensive Security Researcher</strong> — <strong>Red Team Engineer</strong> — <strong>Malware Developer</strong></p>

</div>

<hr/>

<section>

<h2>Identity</h2>

<p>
Anas Labrini is an independent Offensive Security Researcher and Red Team Engineer operating from Morocco. His work is centered on adversary emulation, offensive capability development, and controlled malware research conducted strictly within authorized and regulated environments.
</p>

<p>
His technical foundation originates from low-level system exploration, including Linux internals, networking architecture, and Python-based engineering. This foundation evolved into advanced operational domains such as post-exploitation engineering, command and control architecture, and multi-stage attack simulation frameworks.
</p>

<p>
Current research is focused on designing and implementing realistic offensive systems that accurately replicate modern threat behavior across heterogeneous environments, with particular emphasis on Windows and Linux operational models.
</p>

</section>

<hr/>

<section>

<h2>Operational Scope</h2>

<ul>
<li>Reconnaissance and Intelligence Collection</li>
<li>Initial Access and Exploitation</li>
<li>Privilege Escalation and Lateral Movement</li>
<li>Post-Exploitation Engineering</li>
<li>Persistence and Long-Term Access</li>
<li>Defense Evasion and Anti-Forensics</li>
<li>Command and Control Infrastructure</li>
<li>Malware Development and Behavioral Analysis</li>
<li>Web and Network Attack Simulation</li>
</ul>

</section>

<hr/>

<section>

<h2>Low-Level & Kernel-Oriented Engineering</h2>

<p>
A critical component of his research involves controlled interaction with low-level system layers, extending beyond conventional user-space execution into kernel-adjacent behavior modeling.
</p>

<p>
On Windows platforms, this includes interaction with internal APIs, privilege manipulation primitives, process control mechanisms, and security boundary considerations associated with the NT kernel architecture.
</p>

<p>
On Linux systems, this extends to systemd-based execution control, process lifecycle manipulation, memory-level execution flows, and controlled persistence integration within system-level services.
</p>

<p>
These capabilities support the development of:
</p>

<ul>
<li>Stealth-oriented execution pipelines</li>
<li>Kernel-aware behavioral simulation</li>
<li>Advanced persistence mechanisms aligned with OS internals</li>
<li>Fine-grained runtime control and execution flow manipulation</li>
</ul>

<p>
The objective is not only execution, but accurate behavioral replication of advanced adversaries under controlled research constraints.
</p>

</section>

<hr/>

<section>

<h2>Technical Stack</h2>

<p><strong>Operating Systems</strong></p>
<ul>
<li>Linux — Primary Offensive Platform</li>
<li>Windows — Internal Behavior Analysis and Simulation</li>
</ul>

<p><strong>Programming & Scripting</strong></p>
<ul>
<li>Python</li>
<li>PowerShell</li>
<li>Bash</li>
<li>C (Embedded / Low-Level Contexts)</li>
<li>VBScript</li>
</ul>

<p><strong>Frameworks & Offensive Tooling</strong></p>
<ul>
<li>Metasploit</li>
<li>Cobalt Strike</li>
<li>Empire</li>
<li>Sliver</li>
</ul>

<p><strong>Network & Reconnaissance</strong></p>
<ul>
<li>Nmap</li>
<li>Masscan</li>
<li>Wireshark</li>
<li>Tcpdump</li>
<li>Bettercap</li>
</ul>

<p><strong>Web Security</strong></p>
<ul>
<li>Burp Suite</li>
<li>SQLmap</li>
<li>Ffuf</li>
<li>Gobuster</li>
<li>Feroxbuster</li>
</ul>

<p><strong>Credential Access & AD</strong></p>
<ul>
<li>Hashcat, John the Ripper, Hydra, Medusa</li>
<li>BloodHound, SharpHound, Evil-WinRM, Impacket</li>
</ul>

</section>

<hr/>

<section>

<h2>Selected Projects</h2>

<p>
The following represents a curated subset of developed tools. Each project reflects a focused research domain in offensive security and malware engineering.
</p>

<br/>

<table>
<tr>
<td><strong>CROSSMOS</strong></td>
<td>Modular Windows offensive framework for persistence, C2 communication, and controlled malware simulation.</td>
<td><a href="https://github.com/anaslabrini/crossmos">Access</a></td>
</tr>

<tr>
<td><strong>SpyMorph</strong></td>
<td>Multi-stage Linux execution framework with staged decryption and systemd-based persistence.</td>
<td><a href="https://github.com/anaslabrini/SpyMorph">Access</a></td>
</tr>

<tr>
<td><strong>S-PUP</strong></td>
<td>Cross-platform persistence and surveillance research system with self-recovery architecture.</td>
<td><a href="https://github.com/anaslabrini/S-PUP">Access</a></td>
</tr>

<tr>
<td><strong>AnasC2</strong></td>
<td>Browser-based command and control platform enabling real-time agent interaction.</td>
<td><a href="https://github.com/anaslabrini/AnasC2">Access</a></td>
</tr>

<tr>
<td><strong>AnasHunter</strong></td>
<td>Web attack simulation framework covering injection, brute-force, and DoS testing.</td>
<td><a href="https://github.com/anaslabrini/AnasHunter">Access</a></td>
</tr>

<tr>
<td><strong>AnasOsint</strong></td>
<td>OSINT intelligence framework aggregating multi-source reconnaissance data.</td>
<td><a href="https://github.com/anaslabrini/AnasOsint">Access</a></td>
</tr>

<tr>
<td><strong>AnasRecon</strong></td>
<td>Asset discovery and reconnaissance framework for service enumeration and risk analysis.</td>
<td><a href="https://github.com/anaslabrini/AnasRecon">Access</a></td>
</tr>

<tr>
<td><strong>AnassRedTool</strong></td>
<td>Multi-function Red Team utility for brute-force, scanning, and network operations.</td>
<td><a href="https://github.com/anaslabrini/AnassRedTool">Access</a></td>
</tr>

<tr>
<td><strong>AnaSSHoney</strong></td>
<td>High-interaction SSH honeypot for capturing adversary behavior and credential attempts.</td>
<td><a href="https://github.com/anaslabrini/AnasSSHoney">Access</a></td>
</tr>

</table>

</section>

<hr/>

<section>

<h2>Engineering Approach</h2>

<ul>
<li>Modular and compartmentalized architecture</li>
<li>Multi-stage execution chains</li>
<li>Low-footprint and memory-conscious design</li>
<li>Environment-aware and anti-analysis logic</li>
<li>Layered persistence strategies</li>
<li>Controlled replication of real-world attack behavior</li>
</ul>

</section>

<hr/>

<section>

<h2>Statement</h2>

<p>
The objective is to analyze adversarial behavior across multiple system layers — from user-space execution to kernel-adjacent interactions — in order to reproduce, study, and ultimately strengthen defensive capabilities through realistic simulation.
</p>

</section>

<hr/>

<section>

<h2>Contact</h2>

<p><strong>GitHub:</strong> https://github.com/anaslabrini</p>
<p><strong>Website:</strong> https://anaslabrini.netlify.app</p>

</section>

<hr/>

<section>

<p style="font-size:12px;">
All activities, tools, and research are conducted exclusively within authorized environments for educational, research, and security testing purposes. Unauthorized use is strictly prohibited.
</p>

</section>
