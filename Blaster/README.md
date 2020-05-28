# Blaster | https://tryhackme.com/room/blaster

### [Task 2] Activate Forward Scanners and Launch Proton Torpedoes

#1	How many ports are open on our target system? : `2`

#2	Looks like there's a web server running, what is the title of the page we discover when browsing to it? : `IIS Windows Server`

#3	Interesting, let's see if there's anything else on this web server by fuzzing it. What hidden directory do we discover? : `/retro`

#4	Navigate to our discovered hidden directory, what potential username do we discover? : `wade`

#5	Crawling through the posts, it seems like our user has had some difficulties logging in recently. What possible password do we discover? : `parzival`

#6	Log into the machine via Microsoft Remote Desktop (MSRDP) and read user.txt. What are it's contents? : `THM{HACK_PLAYER_ONE}`

### [Task 3] Breaching the Control Room

#1	When enumerating a machine, it's often useful to look at what the user was last doing. Look around the machine and see if you can find the CVE which was researched on this server. What CVE was it? : `CVE-2019-1388`

#2	Looks like an executable file is necessary for exploitation of this vulnerability and the user didn't really clean up very well after testing it. What is the name of this executable? : `hhupd`

#4	Now that we've spawned a terminal, let's go ahead and run the command 'whoami'. What is the output of running this? : `nt authority\system`

#5	Now that we've confirmed that we have an elevated prompt, read the contents of root.txt on the Administrator's desktop. What are the contents? Keep your terminal up after exploitation so we can use it in task four! : `THM{COIN_OPERATED_EXPLOITATION}`

### [Task 4] Adoption into the Collective

#2	First, let's set the target to PSH (PowerShell). Which target number is PSH? : `2`

#6	Last but certainly not least, let's look at persistence mechanisms via Metasploit. What command can we run in our meterpreter console to setup persistence which automatically starts when the system boots? Don't include anything beyond the base command and the option for boot startup. : `run persistence -X`