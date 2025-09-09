- PowerShell Command to Get Serial Number
```
Get-WmiObject -Class Win32_BIOS | Select-Object SerialNumber
```
```
Get-CimInstance -ClassName Win32_BIOS | Select-Object SerialNumber
```