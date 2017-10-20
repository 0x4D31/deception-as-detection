## Bash History

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
* [honeybits](https://github.com/0x4D31/honeybits)
* [honeyλ](https://github.com/0x4D31/honeyLambda)
* [canarytokens](http://canarytokens.org)
