# Advent of Cyber 2 | https://tryhackme.com/room/adventofcyber2

## [Day 1] Web Exploitation A Christmas Crisis

- What is the name of the cookie used for authentication? : `auth`

- In what format is the value of this cookie encoded? : `Hexadecimal`

- Having decoded the cookie, what format is the data stored in? : `JSON`

- What is the value of Santa's cookie? : `7b22636f6d70616e79223a22546865204265737420466573746976616c20436f6d70616e79222c2022757365726e616d65223a2273616e7461227d`

- What is the flag you're given when the line is fully active? : `THM{MjY0Yzg5NTJmY2Q1NzM1NjBmZWFhYmQy}`

## [Day 2] Web Exploitation The Elf Strikes Back!

- What string of text needs adding to the URL to get access to the upload page? : `?id=ODIzODI5MTNiYmYw`

- What type of file is accepted by the site? : `Image`

- In which directory are the uploaded files stored? : `/uploads/`

- What is the flag in /var/www/flag.txt? : `THM{MGU3Y2UyMGUwNjExYTY4NTAxOWJhMzhh}`

## [Day 3] Web Exploitation Christmas Chaos

- What is the flag? : `THM{885ffab980e049847516f9d8fe99ad1a}`

## [Day 4] Web Exploitation Santa's watching

- wfuzz command : `wfuzz -c -z file,big.txt http://shibes.xyz/api.php?breed=FUZZ`

- What file is there? : `site-log.php`

- What is the flag displayed in the correct post? : `THM{D4t3_AP1}`

## [Day 5] Web Exploitation Someone stole Santa's gift list!

- Without using directory brute forcing, what's Santa's secret login panel? : `/santapanel`

- How many entries are there in the gift database? : `22`

- What did Paul ask for? : `Github Ownership`

- What is the flag? : `thmfox{All_I_Want_for_Christmas_Is_You}`

- What is admin's password? : `EhCNSWzzFP6sc7gB`

## [Day 6] Web Exploitation Be careful with what you wish on a Christmas night

- What vulnerability type was used to exploit the application? : `stored cross-site scripting`

- What query string can be abused to craft a reflected XSS? : `q`

- Run a ZAP (zaproxy) automated scan on the target. How many XSS alerts are in the scan? : `2`

## [Day 7] Networking The Grinch Really Did Steal Christmas

- Open "pcap1.pcap" in Wireshark. What is the IP address that initiates an ICMP/ping? : `10.11.3.2`

- If we only wanted to see HTTP GET requests in our "pcap1.pcap" file, what filter would we use? : `http.request.method == GET`

- Now apply this filter to "pcap1.pcap" in Wireshark, what is the name of the article that the IP address "10.10.67.199" visited? : `reindeer-of-the-week`

- There's a lot of irrelevant data here - Using a filter here would be useful! : `plaintext_password_fiasco`

- Continuing with our analysis of "pcap2.pcap", what is the name of the protocol that is encrypted? : `SSH`

- What is on Elf McSkidy's wishlist that will be used to replace Elf McEager? : `Rubber ducky`

## [Day 8] Networking What's Under the Christmas Tree?

- When was Snort created? : `1998`

- Using Nmap on MACHINE_IP, what are the port numbers of the three services running?  (Please provide your answer in ascending order/lowest -> highest, separated by a comma) : `80,2222,3389`

- Use Nmap to determine the name of the Linux distribution that is running, what is reported as the most likely distribution to be running? : `ubuntu`

- Use Nmap's Network Scripting Engine (NSE) to retrieve the "HTTP-TITLE" of the webserver. Based on the value returned, what do we think this website might be used for? : `blog`
 
## [Day 9] Networking Anyone can be Santa!
 
- Name the directory on the FTP server that has data accessible by the "anonymous" user : `public`

- What script gets executed within this directory? : `backup.sh`

- What movie did Santa have on his Christmas shopping list? : `The Polar Express`

- Re-upload this script to contain malicious data (just like we did in section 9.6. Output the contents of /root/flag.txt! : `THM{even_you_can_be_santa}`

## [Day 10] Networking Don't be sElfish!

- Using enum4linux, how many users are there on the Samba server (10.10.236.5)? : `3`

- Now how many "shares" are there on the Samba server? : `4`

- Use smbclient to try to login to the shares on the Samba server (10.10.236.5). What share doesn't require a password? : `tbfc-santa`

- Log in to this share, what directory did ElfMcSkidy leave for Santa? : `jingle-tune`

## [Day 11] Networking The Rogue Gnome

- What type of privilege escalation involves using a user account to execute commands as an administrator? : `Vertical`

- What is the name of the file that contains a list of users who are a part of the sudo group? : `sudoers`

- What are the contents of the file located at /root/flag.txt? : `thm{2fb10afe933296592}`
