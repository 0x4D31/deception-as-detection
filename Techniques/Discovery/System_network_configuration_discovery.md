# System Network Configuration Discovery

MITRE ATT&CK technique [T1016](https://attack.mitre.org/wiki/Technique/T1016)

Tactic: Discovery

Platform: Windows, Linux, Mac

### Deception Techniques
* Create breadcrumbs or honeytokens to lure the attackers toward the fake systems or network services (i.e. honeypots)
    * Fake entries in DNS, NetBIOS, ARP cache or hosts file
    * Documents/files with deceptive contents

### Useful Tools
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history and hosts entries.