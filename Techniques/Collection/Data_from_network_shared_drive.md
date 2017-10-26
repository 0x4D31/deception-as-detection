# Data from Network Shared Drive

MITRE ATT&CK technique [T1039](https://attack.mitre.org/wiki/Technique/T1039)

Tactic: Collection

Platform: Windows, Linux, Mac

### Deception Techniques
* Create fake network shares, or create fake directories/files (i.e. honeyfiles) in real network shares, and monitor access to them using the OS file/folder auditing or FIM tools.
* Create decoy files or documents (beacons) that phone home when opened.

### Useful Tools
* [honeyλ](https://github.com/0x4D31/honeyLambda) - Serverless application designed to create and monitor URL honeytokens (i.e. fake HTTP endpoints) automatically
* [canarytokens](http://canarytokens.org)
