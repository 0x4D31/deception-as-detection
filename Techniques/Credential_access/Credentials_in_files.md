# Credentials in Files

MITRE ATT&CK technique [T1081](https://attack.mitre.org/wiki/Technique/T1081)

Tactic: Credential Access

Platform: Windows, Linux, Mac

### Deception Techniques
* Create documents and files containing fake credentials (i.e. honey accounts)
  * Configuration, backup and connection files such as RDP, VPN, and AWS credentials file
  * Fake credentials in browser password manager
  * bash_history entries containing fake credentials, e.g.:
```
mysql -h 192.168.1.66 -P 3306 -u dbadmin -p12345 -e "show databases"
ftp ftp://backup:b123@192.168.1.66:2121
sshpass -p '123456' ssh -p 2222 root@192.168.1.66
export AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
export AWS_SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
```


### Useful Tools
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.