# Network Sniffing

MITRE ATT&CK technique [T1040](https://attack.mitre.org/wiki/Technique/T1040)

Tactic: Credential Access

Platform: Windows, Linux, Mac

### Deception Techniques
* Inject honeytokens such as fake URLs and credentials into the network traffic
* Open network connections to fake systems or network services (i.e. honeypots)

### Useful Tools
* [Beeswarm](https://github.com/honeynet/beeswarm) - It intentionally leaks credentials in the network traffic and then looks for the unexpected reuse of these honey credentials. Beeswarm operates by deploying fake end-user systems (clients) and services (honeypots).