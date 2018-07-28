# Bandit

### Level -1

Simple ssh.

```
ssh bandit0@bandit.labs.overthewire.org
```
Password: *bandit0*

### Level 0

```
bandit0@melinda:~$ ls  
readme
bandit0@melinda:~$ cat readme 
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```
Password: *boJ9jbbUNNfktd78OOpsqOltutMc3MY1*

### Level 1

Filename with name '-'.

```
bandit1@melinda:~$ cat ~/-    
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
bandit1@melinda:~$ cat <-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
Password: *CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9*

### Level 2

Filename with spaces.

```
bandit2@melinda:~$ cat "spaces in this filename"  
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```
Password: *UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK*

### Level 3

```
bandit3@melinda:~$ ls
inhere
bandit3@melinda:~$ cd inhere/
bandit3@melinda:~/inhere$ ls -latr
total 12
drwxr-xr-x 3 root    root    4096 Nov 14  2014 ..
-rw-r----- 1 bandit4 bandit3   33 Nov 14  2014 .hidden
drwxr-xr-x 2 root    root    4096 Nov 14  2014 .
bandit3@melinda:~/inhere$ cat .hidden 
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```
Password: *pIwrPrtPN36QITSp3EQaw936yaFoFgAB*

### Level 4

```
bandit4@melinda:~/inhere$ file ./-file0*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@melinda:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```
Password: *koReBOKuIDDepwhWk7jZC0RTdopnAYKh*

### Level 5

```
bandit5@melinda:~/inhere$ find . -size 1033c
./maybehere07/.file2
bandit5@melinda:~/inhere$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```
Password: *DXjZPULLxYr17uwoI01bNLQbtFemEgo7*

### Level 6

```
bandit6@melinda:/$ cd /
bandit6@melinda:/$ find . -user bandit7 -group bandit6
bandit6@melinda:/$ cat ./var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```
Password: *HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs*

### Level 7

```
bandit7@melinda:~$ cat data.txt | grep millionth
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```
Password: cvX2JJa4CFALtqS87jk27qwqGhBM9plV

### Level 8

```
bandit8@melinda:~$ cat data.txt | sort | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
```
Password: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

### Level 9

```
bandit9@melinda:~$ strings data.txt  | grep "^="
========== password
========== ism
========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
```
Password: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

### Level 10

```
bandit10@melinda:~$  base64 -d data.txt 
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```
Password: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

### Level 11

```
bandit11@melinda:~$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
```
Password: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

### Level 12

Use `xxd -r` to revert the hexdump to its original form. Then use mv, bunzip2, bunzip and tar multiple times till you reach the end.
```
bandit12@melinda:/tmp/alex$ cat data8
The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
```
Password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

### Level 13

```
alx@conjecture:~$ scp -P 2220 bandit13@bandit.labs.overthewire.org:~/sshkey.private .
alx@conjecture:~$ chmod 600 sshkey.private 
alx@conjecture:~$ ssh -p 2220 -i sshkey.private bandit14@bandit.labs.overthewire.org
```
Password: (none)

### Level 14

```
bandit14@melinda:~$ cat /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
bandit14@melinda:~$ nc localhost 30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr
```
Password: BfMYroe26WYalil77FoDi9qh59eK5xNr

### Level 15

```
bandit15@bandit:~$ openssl s_client -connect localhost:30001 -ign_eof
```
Password: cluFn7wTiGryunymYOu4RcffSxQluehd

### Level 16

```
bandit16@bandit:~$ nmap -A -p 31000-32000 localhost
bandit16@bandit:~$ openssl s_client -connect localhost:31790

```
Password: [Private Key]

### Level 17

```
bandit17@bandit:~$ diff passwords.new passwords.old 
```
Password:kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

### Level 18
Login without triggering bash, thus skipping bashrc.
```
alex@Conjecture:~$ ssh -p 2220 -t bandit18@bandit.labs.overthewire.org /bin/sh
$ cat readme
```
Password: IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

### Level 19

```
bandit19@bandit:~$ ./bandit20-do cat /etc/bandit_pass/bandit20 
```
Password: GbKksEFF4yrVs6il55v6gwY5aVje5f0j

### Level 20
Use tmux to create two new windows. Run a nc server in one of them and use the uuid binary in the other.
```
bandit20@bandit:~$ nc -l 5000
GbKksEFF4yrVs6il55v6gwY5aVje5f0j

bandit20@bandit:~$ ./suconnect 5000
```
Password: gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr

### Level 21

```
bandit21@bandit:~$ cat /etc/cron.d/cronjob_bandit22
bandit21@bandit:~$ less /usr/bin/cronjob_bandit22.sh
bandit21@bandit:~$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```
Password: Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI
