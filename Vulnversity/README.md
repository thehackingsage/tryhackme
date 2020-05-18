# Vulnversity | https://tryhackme.com/room/vulnversity

### [Task 2] Reconnaissance

#2	Scan the box, how many ports are open? : ```6```

#3	What version of the squid proxy is running on the machine? : ```3.5.12```

#4	How many ports will nmap scan if the flag -p-400 was used? : ```400```

#5	Using the nmap flag -n what will it not resolve? : ```DNS```

#6	What is the most likely operating system this machine is running? : ```Ubuntu```

#7	What port is the web server running on? : ```3333```

### [Task 3] Locating directories using GoBuster

#2	What is the directory that has an upload form page? : ```/internal/```

### [Task 4] Compromise the webserver

#1	Try upload a few file types to the server, what common extension seems to be blocked? : ```.php```
	
#3	what extension is allowed? : ```.phtml```

#5	What user was running the web server? : ```bill```

#6	What is the user flag? : ```8bd7992fbe8a6ad22a63361004cfcedb```

### [Task 5] Privilege Escalation

#1	On the system, search for all SUID files. What file stands out? : ```/bin/systemctl```

#2	Its challenge time! We have guided you through this far, are you able to exploit this system further to escalate your privileges and get the final answer? Become root and get the last flag (/root/root.txt) : ```a58ff8579f0a9270368d33a9966c7fd5```
