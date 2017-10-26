# Data from Removable Media

MITRE ATT&CK technique [T1025](https://attack.mitre.org/wiki/Technique/T1025)

Tactic: Collection

Platform: Windows, Linux, Mac

### Deception Techniques
* Create decoy files or documents (beacons) that phone home when opened.
* Create emulated or virtual USB devices and monitor access to them (e.g. using Windows Removable Storage Auditing)
* Create files containing deceptive content and breadcrumbs to lure the attacker toward your honeypots.

### Useful Tools
* [Ghost USB Honeypot](https://github.com/honeynet/ghost-usb-honeypot) - It emulates a USB storage device to detect malwares that use such devices for propagation. Ghost supports Windows XP 32 bit and Windows 7 32 bit.
* [honeyλ](https://github.com/0x4D31/honeyLambda) - Serverless application designed to create and monitor URL honeytokens (i.e. fake HTTP endpoints) automatically
* [canarytokens](http://canarytokens.org)