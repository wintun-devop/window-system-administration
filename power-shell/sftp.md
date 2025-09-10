### sshd server service check - Window PowerShell
```
Get-WindowsCapability -Online | ? Name -like 'OpenSSH.Ser*'
```

### sshd service allow on firewall - Window PowerShell
```
Set-Service -Name sshd -StartupType 'Automatic'
```
```
Start-Service sshd
```

###  sshd service status check - Window PowerShell
```
Get-NetFirewallRule -Name *OpenSSH-Server* |select Name, DisplayName, Description, Enabled
```

### ssh port checking on network level(command prompt)
```
netstat -na| find ":22"
```
