# Replication Through Removable Media

MITRE ATT&CK technique [T1091](https://attack.mitre.org/wiki/Technique/T1091)

Tactic: Lateral Movement

Platform: Windows

### Deception Techniques
* Create emulated or virtual USB devices and monitor access to them (e.g. using Windows Removable Storage Auditing)

### Useful Tools
* [Ghost USB Honeypot](https://github.com/honeynet/ghost-usb-honeypot) - It emulates a USB storage device to detect malwares that use such devices for propagation. Ghost supports Windows XP 32 bit and Windows 7 32 bit.
* [USB/IP](http://usbip.sourceforge.net/) project