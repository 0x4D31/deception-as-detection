# Network Service Scanning

MITRE ATT&CK technique [T1046](https://attack.mitre.org/wiki/Technique/T1046)

Tactic: Discovery

Platform: Windows, Linux, Mac

### Deception Techniques
* Set up fake network services
* Create breadcrumbs or honeytokens to lure the attackers toward the fake network services (i.e. honeypots)
    * Fake entries in ARP cache, hosts file, etc.
    * Documents/files with deceptive contents

### Useful Tools
* [Glutton](https://github.com/mushorg/glutton) - All eating honeypot
* [Dionaea](https://github.com/DinoTools/dionaea) - A low-interaction honeypot to trap malware exploiting vulnerabilities exposed by services offerd to a network. Dionaea emulates several protocols such as smb, sip, ftp, tftp, mssql, mysql, http, and uses libemu to detect shellcodes.
* [Conpot](https://github.com/mushorg/conpot) - ICS/SCADA honeypot
* Snare & Tanner - Successors to [Glastopf](https://github.com/mushorg/glastopf) web application honeypot.
    * [SNARE](https://github.com/mushorg/snare) - Super Next generation Advanced Reactive honEypot
    * [Tanner](https://github.com/mushorg/tanner) - Evaluating SNARE events
* [Cowrie](https://github.com/micheloosterhof/cowrie) - A medium interaction SSH and Telnet honeypot designed to log brute force attacks and the shell interaction performed by the attacker.
* [Amun](https://github.com/zeroq/amun) - A low-interaction honeypot, following the concepts of Nepenthes but extending it with more sophisticated emulation and easier maintenance.
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
* [MazeRunner](https://community.cymmetria.com/) community edition

### Useful Resources:
* [awesome-honeypots](https://github.com/paralax/awesome-honeypots)