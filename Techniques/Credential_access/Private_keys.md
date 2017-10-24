# Private Keys

MITRE ATT&CK technique [T1145](https://attack.mitre.org/wiki/Technique/T1145)

Tactic: Credential Access

Platform: Windows, Linux, Mac

### Deception Techniques
* Create fake private keys (i.e. honeyfiles) and monitor access to them using go-audit, auditd or a File Integrity Monitoring (FIM) 
* Create files or documents containing deceptive content and breadcrumbs (e.g. keys for connecting to SSH honeypots) to lure the attacker toward your honeypots.
    * Fake entries in ~/.ssh/known_hosts, e.g.:
```
192.168.1.66 ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAEXAMPLE
```

### Useful Tools
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
* [go-audit](https://github.com/slackhq/go-audit) - An alternative to the auditd daemon, with json output.

### Useful Resources
* [Catching attackers with go-audit and a logging pipeline](https://summitroute.com/blog/2016/12/25/Catching_attackers_with_go-audit_and_a_logging_pipeline/)