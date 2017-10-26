# Remote Services

MITRE ATT&CK technique [T1021](https://attack.mitre.org/wiki/Technique/T1021)

Tactic: Lateral Movement

Platform: Windows, Linux, Mac

### Deception Techniques
* Set up fake network services or protocols such as Telnet, SSH and VNC
* Create breadcrumbs or honeytokens to lure the attackers toward the fake network services (i.e. honeypots)
    * Documents/files with deceptive contents and breadcrumbs
    * Manipulate bash_history with fake entries, e.g.:
```
sshpass -p '123456' ssh -p 2222 root@192.168.1.66
```

### Useful Tools
* [Cowrie](https://github.com/micheloosterhof/cowrie) - A medium interaction SSH and Telnet honeypot designed to log brute force attacks and the shell interaction performed by the attacker, with SFTP and SCP support.
* [Glutton](https://github.com/mushorg/glutton) - All eating honeypot
* [HonSSH](https://github.com/tnich/honssh) - It is designed to be used in conjunction with a high-interaction honeypot. HonSSH sits between the attacker and the honeypot and creates two separate SSH conncetions.
* [SSHHiPot](https://github.com/magisterquis/sshhipot) - A logging SSH proxy that can be used as an high-interaction SSH honeypot.
* [Wetland](https://github.com/ohmyadd/wetland) - A docker based high-interaction SSH honeypot
* [vnclowpot](https://github.com/magisterquis/vnclowpot) - Low-interaction VNC honeypot
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
* [Sysdig](https://github.com/draios/sysdig)

## Useful Resources
* [Bifrozt high interaction SSH honeypot](https://www.honeynet.org/node/1191)