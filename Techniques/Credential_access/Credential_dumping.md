# Credential Dumping

MITRE ATT&CK technique [T1003](https://attack.mitre.org/wiki/Technique/T1003)

Tactic: Credential Access

Platform: Windows

### Deception Techniques
* Inject fake credentials into LSASS (i.e. honey hashes)
* Create Kerberoast Service Account honeytoken
* Create files containing fake credentials (i.e. honey accounts)
  * Configuration, backup and connection files such as RDP, VPN, and AWS credentials file
  * Fake credentials in browser password manager

### Useful Tools
* [New-HoneyHash.ps1](https://github.com/EmpireProject/Empire/blob/master/data/module_source/management/New-HoneyHash.ps1) - Inject artificial credentials into LSASS. New-HoneyHash is a simple wrapper for advapi32!CreateProcessWithLogonW that specifies the LOGON_NETCREDENTIALS_ONLY flag.
* [DCEPT](https://github.com/secureworks/dcept) (Domain Controller Enticing Password Tripwire) - A tool for deploying and detecting use of Active Directory honeytokens
* [honeybits-win](https://github.com/0x4D31/honeybits-win) - The windows version of [honeybits](https://github.com/0x4D31/honeybits) that supports creating fake credentials in Windows Credential Manager.

### Useful Resources
* [Detecting Kerberoasting Activity Part 2 – Creating a Kerberoast Service Account Honeypot](https://adsecurity.org/?p=3513)
* [Detecting Mimikatz Use On Your Network](https://isc.sans.edu/forums/diary/Detecting+Mimikatz+Use+On+Your+Network/19311/)
* [DCEPT](https://www.secureworks.com/blog/dcept): An Open-Source Honeytoken Tripwire
* [Dealing with credential theft](https://dfirblog.wordpress.com/2015/11/24/protecting-windows-networks-dealing-with-credential-theft/)
* [Busting the Honeypot – Is there really a way for attackers to detect deception](https://www.topspinsec.com/blog/busting-honeypot-really-way-attackers-detect-deception/)
* [MimikatzHoneyToken](https://github.com/SMAPPER/MimikatzHoneyToken) - A logon script used to detect the theft of credentials by tools such as Mimikatz. This script is an AutoIT logon script that launches cmd.exe as a fake user account. It is intended to be ran as a logon script on windows systems.