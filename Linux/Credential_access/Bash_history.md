# Bash History

MITRE ATT&CK technique [T1139](https://attack.mitre.org/wiki/Technique/T1139)

### Deception Techniques
* Manipulate bash_history with fake entries (honeytokens and breadcrumbs)

```
sshpass -p '123456' ssh -p 2222 root@192.168.1.66
ftp ftp://backup:b123@192.168.1.66:2121
mysql -h 192.168.1.66 -P 3306 -u dbadmin -p12345 -e "show databases"
scp -P 2222 root@192.168.1.66:/var/db/backup.tar.gz /tmp/backup.tar.gz
```

### Useful Tools
* [honeybits](https://github.com/0x4D31/honeybits) - A tool designed to enhance the effectiveness of honeypots by spreading breadcrumbs & honeytokens across the system. Currently supports creating honeyfiles and several breadcrumbs including fake bash_history entries.
* [honeyλ](https://github.com/0x4D31/honeyLambda) - Serverless application designed to create and monitor URL honeytokens (i.e. fake HTTP endpoints) automatically
* [canarytokens](http://canarytokens.org)
