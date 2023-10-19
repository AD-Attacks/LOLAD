---
description: How to enumerate users using net user command
---

# Users



<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

### Enumerate Local Users using Net Command

{% embed url="https://learn.microsoft.com/en-us/troubleshoot/windows-server/networking/net-commands-on-operating-systems" %}

### Enumerate Domain Users using Net Command

```powershell
net user /domain
```

### Add a new local User using Net command

```
net user rfs rfs!rfs /add
```



### Add a Domain local User using Net command

```
net user rfs rfs!rfs /add /domain
```
