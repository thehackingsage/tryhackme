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

## [Day 12] Networking Ready, set, elf.

- What is the version number of the web server? : `9.0.17`

- What CVE can be used to create a Meterpreter entry onto the machine? (Format: CVE-XXXX-XXXX) : `CVE-2019-0232`

- What are the contents of flag1.txt : `thm{whacking_all_the_elves}`

##  [Day 13] Special by John Hammond Coal for Christmas

- What old, deprecated protocol and service is running? - `telnet`

- What credential was left for you? : `clauschristmas`

- What distribution of Linux and version number is this server running? : `Ubuntu 12.04`

- Who got here first? : `grinch`

- What is the verbatim syntax you can use to compile, taken from the real C source code comments? : `gcc -pthread dirty.c -o dirty -lcrypt`

- What "new" username was created, with the default operations of the real C source code? : `firefart`

- What is the MD5 hash output? : `8b16f00dd3b51efadb02c1df7f8427cc`

## [Day 14] Special by TheCyberMentor Where's Rudolph?

- What URL will take me directly to Rudolph's Reddit comment history? : `https://www.reddit.com/user/IGuidetheClaus2020/comments/`

- According to Rudolph, where was he born? : `chicago`

- Rudolph mentions Robert.  Can you use Google to tell me Robert's last name? : `may`

- On what other social media platform might Rudolph have an account? : `twitter`

- What is Rudolph's username on that platform? : `IGuideClaus2020`

- What appears to be Rudolph's favorite TV show right now? : `bachelorette`

- Based on Rudolph's post history, he took part in a parade.  Where did the parade take place? : `chicago`

- Okay, you found the city, but where specifically was one of the photos taken? : `41.891815, -87.624277`

- Did you find a flag too? : `{FLAG}ALWAYSCHECKTHEEXIFD4T4`

- Has Rudolph been pwned? What password of his appeared in a breach? : `spygame`

- Based on all the information gathered.  It's likely that Rudolph is in the Windy City and is staying in a hotel on Magnificent Mile.  What are the street numbers of the hotel address? : `540`

## [Day 15] Scripting There's a Python in my stocking!

- What's the output of True + True? : `2`

- What's the database for installing other peoples libraries called? : `PyPi`

- What is the output of bool("False")? : `True`

- What library lets us download the HTML of a webpage? : `Requests`

- What is the output of the program provided in "Code to analyse for Question 5" in today's material? : `[1, 2, 3, 6]`

- What causes the previous task to output that? : `Pass by reference`

## [Day 16] Scripting Help! Where is Santa?

- What is the port number for the web server? : `8000`

- Without using enumerations tools such as Dirbuster, what is the directory for the API?  (without the API key) : `/api/`

- Where is Santa right now? : `Winter wonderland, Hyde Park, London`

- Find out the correct API key. Remember, this is an odd number between 0-100. After too many attempts, Santa's Sled will block you. : `57`

## [Day 17] Reverse Engineering ReverseELFneering

- What is the value of local_ch when its corresponding movl instruction is called (first if multiple)? : `1`

- What is the value of eax when the imull instruction is called? : `6`

- What is the value of local_4h before eax is set to 0? : `6`

## [Day 18] Reverse Engineering The Bits of Christmas

- What is Santa's password? : `santapassword321`

- Now that you've retrieved this password, try to login...What is the flag? : `thm{046af}`

## [Day 19] Special by Tib3rius The Naughty or Nice List

- What is Santa's password? : `be good for goodness sake!`

- What is the challenge flag? : `THM{EVERYONE_GETS_PRESENTS}`

## [Day 20] Blue Teaming PowershELlF to the rescue

- Search for the first hidden elf file within the Documents folder. Read the contents of this file. What does Elf 1 want? : `2 front teeth`

- Search on the desktop for a hidden folder that contains the file for Elf 2. Read the contents of this file. What is the name of that movie that Elf 2 wants? : `scrooged`

- Search the Windows directory for a hidden folder that contains files for Elf 3. What is the name of the hidden folder? (This command will take a while) : `3lfthr3e`

- How many words does the first file contain? : `9999`

- What 2 words are at index 551 and 6991 in the first file? : `Red Ryder`

- This is only half the answer. Search in the 2nd file for the phrase from the previous question to get the full answer. What does Elf 3 want? (use spaces when submitting the answer) : `red ryder bb gun`

## [Day 21] Blue Teaming Time for some ELForensics

- Read the contents of the text file within the Documents folder. What is the file hash for db.exe? : `596690FFC54A86101932856E6A78E3A1`

- What is the file hash of the mysterious executable within the Documents folder? : `5F0375O1FB542AD2D9B06EB12AED09F0`

- Using Strings find the hidden flag within the executable? : `THM{f6187e6cbeb1214139ef313e108cb6f9}`

- What is the flag that is displayed when you run the database connector file? : `THM{088731ddc7b9fdeccaed982b07c297c}`

## [Day 22] Blue Teaming Elf McEager becomes CyberElf
 
- What is the password to the KeePass database? : `thegrinchwashere`
 
- What is the encoding method listed as the 'Matching ops'? : `base64`

- What is the decoded password value of the Elf Server? : `sn0wM4n!`

- What is the decoded password value for ElfMail? : `ic3Skating`

- Decode the last encoded value. What is the flag? : `THM{657012dcf3d1318dca0ed864f0e70535}`

## [Day 23] Blue Teaming The Grinch strikes again!

- Decrypt the fake 'bitcoin address' within the ransom note. What is the plain text value? : `nomorebestfestivalcompany`

- At times ransomware changes the file extensions of the encrypted files. What is the file extension for each of the encrypted files? : `.grinch`

- What is the name of the suspicious scheduled task? : `opidsfsdf`

- Inspect the properties of the scheduled task. What is the location of the executable that is run at login? : `C:\Users\Administrator\Desktop\opidsfsdf.exe`

- There is another scheduled task that is related to VSS. What is the ShadowCopyVolume ID? : `7a9eea15-0000-0000-0000-010000000000`

- Assign the hidden partition a letter. What is the name of the hidden folder? : `confidential`

- Right-click and inspect the properties for the hidden folder. Use the 'Previous Versions' tab to restore the encrypted file that is within this hidden folder to the previous version. What is the password within the file? : `m33pa55w0rdIZseecure!`
