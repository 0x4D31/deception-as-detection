# Email Collection

MITRE ATT&CK technique [T1114](https://attack.mitre.org/wiki/Technique/T1114)

Tactic: Collection

Platform: Windows

### Deception Techniques
* Create fake Outlook storage or cache files .pst and .ost
    * Fake emails containing deceptive content and breadcrumbs to lure the attacker toward your honeypots.
    * Fake emails containing decoy documents or URL honeytokens (beacons) that phone home when opened/clicked.


### Useful Tools
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
* [honeyλ](https://github.com/0x4D31/honeyLambda) - Serverless application designed to create and monitor URL honeytokens (i.e. fake HTTP endpoints) automatically
* [canarytokens](http://canarytokens.org)