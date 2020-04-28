# Check the powershell Version. Ansible recommned to install latest version of powershell.  
>> $PSVersionTable.PSVersion.

# If you don't have latest version of powershell download and run below script from repo.
"Upgrading PowerShell and .NET Framework.ps1"

# Configuring & Enable WinRM - 
Download and excutute on "ConfigureRemotingForAnsible.ps1" remote machine.
check Vm listner status using below commond
>> winrm enumerate winrm/config/Listener
check Winrm service on machine
>> winrs -r:http://$hostname:5985/wsman -u:$username -p:password ipconfig

