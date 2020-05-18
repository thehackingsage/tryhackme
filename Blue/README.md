# Blue | https://tryhackme.com/room/blue

### [Task 1] Recon

#2	How many ports are open with a port number under 1000? : ```3```

#3	What is this machine vulnerable to? (Answer in the form of: ms??-???, ex: ms08-067) : ```ms17-010```

### [Task 2] Gain Access

#2	Find the exploitation code we will run against the machine. What is the full path of the code? (Ex: exploit/........) : ```exploit/windows/smb/ms17_010_eternalblue```

#3	Show options and set the one required value. What is the name of this value? (All caps for submission) : ```RHOST```

### [Task 3] Escalate

#1	If you haven't already, background the previously gained shell (CTRL + Z). Research online how to convert a shell to meterpreter shell in metasploit. What is the name of the post module we will use? (Exact path, similar to the exploit we previously selected) : ```post/multi/manager/shell_to_meterpreter```

#2	Select this (use MODULE_PATH). Show options, what option are we required to change? (All caps for answer) : ```SESSION```

### [Task 4] Cracking

#1	Within our elevated meterpreter shell, run the command 'hashdump'. This will dump all of the passwords on the machine as long as we have the correct privileges to do so. What is the name of the non-default user? : ```jon```

#2	Copy this password hash to a file and research how to crack it. What is the cracked password? : ```azlgfna22```

### [Task 5] Find flags!

#1	Flag1? (Only submit the flag contents {CONTENTS}) : ```access_the_machine```

#2	Flag2? *Errata: Windows really doesn't like the location of this flag and can occasionally delete it. It may be necessary in some cases to terminate/restart the machine and rerun the exploit to find this flag. This relatively rare, however, it can happen. : ```sam_database_elevated_access```

#3	flag3? : ```admin_documents_can_be_valuable```