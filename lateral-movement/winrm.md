---
description: WinRM for Lateral Movement
---

# WinRM

WinRM is a Microsoft technology that enables remote management and automation of Windows-based systems. It's especially valuable in enterprise environments where IT administrators need to manage multiple Windows servers and workstations.

WinRM, or Windows Remote Management, is a legitimate Windows management tool that can be misused for lateral movement by threat actors during cyberattacks.

```
PS C:\htb> Test-NetConnection -ComputerName DATABASE01 -Port 5985

ComputerName     : DATABASE01
RemoteAddress    : 192.168.1.101
RemotePort       : 5985
InterfaceAlias   : Ethernet0
SourceAddress    : 192.168.1.100
TcpTestSucceeded : True
```

```
PS C:\htb> $Session = New-PSSession -ComputerName DATABASE01
```

{% code overflow="wrap" %}
```powershell
PS C:\htb> Copy-Item -Path C:\samplefile.txt -ToSession $Session -Destination C:\Users\Administrator\Desktop\
```
{% endcode %}

{% code overflow="wrap" %}
```powershell
PS C:\htb> Copy-Item -Path "C:\Users\Administrator\Desktop\DATABASE.txt" -Destination C:\ -FromSession $Session
```
{% endcode %}
