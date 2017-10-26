# Automated Collection

MITRE ATT&CK technique [T1119](https://attack.mitre.org/wiki/Technique/T1119)

Tactic: Collection

Platform: Windows, Linux, Mac

### Deception Techniques
* Create fake directories and files (i.e. honeyfiles) and monitor access to them using go-audit, auditd, File Integrity Monitoring (FIM) tool, or the OS file/folder auditing.
* Create decoy files or documents (beacons) that phone home when opened.
* Create files containing deceptive content and breadcrumbs to lure the attacker toward your honeypots.

### Useful Tools
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
* [go-audit](https://github.com/slackhq/go-audit) - An alternative to the auditd daemon, with json output.
* [honeyλ](https://github.com/0x4D31/honeyLambda) - Serverless application designed to create and monitor URL honeytokens (i.e. fake HTTP endpoints) automatically
* [canarytokens](http://canarytokens.org)

### Useful Resources
* [Catching attackers with go-audit and a logging pipeline](https://summitroute.com/blog/2016/12/25/Catching_attackers_with_go-audit_and_a_logging_pipeline/)
* [Using Windows File Auditing to Detect Honeyfile Access](https://labs.mwrinfosecurity.com/blog/using-windows-file-auditing-to-detect-honeyfile-access/)
* [Automating the Generation of Enticing Text Content for High-Interaction Honeyfiles](https://scholarspace.manoa.hawaii.edu/handle/10125/41897)
* [Canary Files](http://sdiwc.net/digital-library/download.php?id=00000551.pdf): generating fake files to detect critical data loss from complex computer networks
* [Design requirements for generating deceptive content to protect document repositories](http://ro.ecu.edu.au/cgi/viewcontent.cgi?article=1055&context=isw)