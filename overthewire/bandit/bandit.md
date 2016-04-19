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
