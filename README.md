# Horizon-View-Pool-Tools
PowerShell with PowerCLI scripts to manages VMs in a Horizon View Pool</br>
These tools are designed to;</br>
1. Power Down a Horizon View Pool</br>
2. Power Up a Horizon View Pool</br>
3. Refresh a Horizon View Pool</br>
</br>
#Setup</br>
Script must be run on Connection Broker (Horizon View Connection Server) as View admin user.</br>
The Connection Broker must have both PowerShell, VMMware PowerCLI and View PowerCLI installed on it.</br>
</br>
# How to install PowerShell, VMWare PowerCLI and View PowerCLI</br>
PowerShell comes a part of Windows 2008, 2012 and 2016</br>
View PowerCLI comes as part of the Horizon View Connection Server install</br>
Goto VMWare.com and download VMWare PowerCLI 5.5</br>
Install VMWare PowerCLI 5.5</br>
</br>
# How to configure the script</br>
Edit the PowerShell script and enter the informion relevent to your orgisnation</br>
$SmtpClient.host</br>
$MailMessage.from</br>
$MailMessage.To.add</br>
</br>
# How to run the script</br>
1. Open Powershell command windows</br>
2. .\View_PowerDown_Pool.ps1 -Pool Pool_id</br>
3. .\View_Refresh_Pool.ps1 -Pool Pool_id</br>
2. .\View_PowerUp_Pool.ps1 -Pool Pool_id</br>
</br>
# Note</br>
PowerDown and PowerUp modifies 'Number of space (powered on) desktops:'</br>
Will only work if the pool setting 'Remote Desktop Power Policy:' is set to 'Power off'</br>
