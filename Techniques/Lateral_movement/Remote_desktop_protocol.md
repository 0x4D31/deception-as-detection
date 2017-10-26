# Remote Desktop Protocol

MITRE ATT&CK technique [T1076](https://attack.mitre.org/wiki/Technique/T1076)

Tactic: Lateral Movement

Platform: Windows

### Deception Techniques
* Set up fake RDP services
* Create fake RDP connection files
* Create files or documents containing deceptive contents and breadcrumbs to lure the attacker toward your RDP honeypot (emulated or real)

### Useful Tools
* [RDPY](https://github.com/citronneur/rdpy) - A pure Python implementation of the Microsoft RDP (Remote Desktop Protocol) protocol (client and server side).
* [xrdp](https://github.com/neutrinolabs/xrdp) - An open source RDP server
* [Tom's Honeypot](http://labs.inguardians.com/tomshoneypot.html) - A very simple honeypot with RDP support
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.

## Useful Resources
* [RDP Honeypot on Amazon EC2 Virtual Server](https://samsclass.info/123/proj10/rdp-honeypot.htm)