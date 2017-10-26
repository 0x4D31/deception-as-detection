# Commonly Used Port

MITRE ATT&CK technique [T1043](https://attack.mitre.org/wiki/Technique/T1043)

Tactic: Command and Control

Platform: Windows, Linux, Mac

### Deception Techniques
* Set up network sinkholes (fake network services or protocols such as HTTP, HTTPS, FTP, SMTP and DNS).
    * Using internal DNS servers you would be able to redirect all known malicious domains to the internal network sinkhole. This would allow for the detection of internal infected machines as well as preventing the infected machines from communicating with the C&C server.

### Useful Tools
* [HoneySink](http://www.honeynet.org/node/773) - A network sinkhole for DNS, HTTP, FTP and IRC protocols
* [netsarlacc](https://github.com/ciscocsirt/netsarlacc) - A high performance enterprise HTTP (and SMTP) sinkhole designed to be used by corporate SOC or IR teams. netsarlacc is meant to work in conjunction with existing blocking / captive portal / quarantining / redirecting technologies like DNS RPZ.
* [UDPot](https://github.com/jekil/UDPot)
* [ApateDNS](https://www.fireeye.com/services/freeware/apatedns.html) - As a phony DNS server, ApateDNS spoofs DNS responses to a user-specified IP address by listening on UDP port 53 on the local machine.
* [INetSim](http://www.inetsim.org/downloads.html) - A tool for simulating common internet services including HTTP(S), FTP(S), POP3(S), SMTP(S), DNS, TFTP, IRC and etc.