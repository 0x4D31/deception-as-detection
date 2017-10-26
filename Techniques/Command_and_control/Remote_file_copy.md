# Remote File Copy

MITRE ATT&CK technique [T1105](https://attack.mitre.org/wiki/Technique/T1105)

Tactic: Lateral Movement, Command and Control

Platform: Windows, Linux, Mac

### Deception Techniques
* Set up fake network services or protocols such as FTP, SFTP and SCP
* Create breadcrumbs or honeytokens to lure the attackers toward the fake network services (i.e. honeypots)
    * Documents/files with deceptive contents and breadcrumbs
    * Manipulate bash_history with fake entries, e.g.:
```
ftp ftp://backup:b123@192.168.1.66:2121
scp -P 2222 root@192.168.1.66:/var/db/backup.tar.gz /tmp/backup.tar.gz
```
* Using internal DNS servers you would be able to redirect all known malicious domains to the internal network sinkhole. This would allow for the detection of internal infected machines as well as preventing the infected machines from communicating with the C&C server.

### Useful Tools
* [Cowrie](https://github.com/micheloosterhof/cowrie) - A medium interaction SSH and Telnet honeypot designed to log brute force attacks and the shell interaction performed by the attacker, with SFTP and SCP support.
* [Dionaea](https://github.com/DinoTools/dionaea) - A low-interaction honeypot to trap malware exploiting vulnerabilities exposed by services offerd to a network. Dionaea emulates several protocols such as smb, sip, ftp, tftp, mssql, mysql, http, and uses libemu to detect shellcodes.
* [HoneySink](http://www.honeynet.org/node/773) - A network sinkhole for DNS, HTTP, FTP and IRC protocols
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
