# Network Share Discovery

MITRE ATT&CK technique [T1135](https://attack.mitre.org/wiki/Technique/T1135)

Tactic: Discovery

Platform: Windows, Mac

### Deception Techniques
* Create fake network shares, or create fake directories/files (i.e. honeyfiles) in real network shares, and monitor access to them using the OS file/folder auditing or FIM tools.
* Create decoy files or documents (beacons) that phone home when opened.

### Useful Tools
* [honeyλ](https://github.com/0x4D31/honeyLambda) - Serverless application designed to create and monitor URL honeytokens (i.e. fake HTTP endpoints) automatically
* [canarytokens](http://canarytokens.org)
