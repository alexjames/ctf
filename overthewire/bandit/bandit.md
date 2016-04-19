# Bandit

### Level 0

Simple ssh.

```
ssh bandit0@bandit.labs.overthewire.org
```
Password: *bandit0*

### Level 1

```
bandit0@melinda:~$ ls  
readme
bandit0@melinda:~$ cat readme 
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```
Password: *boJ9jbbUNNfktd78OOpsqOltutMc3MY1*

### Level 2

Filename with name '-'.

```
bandit1@melinda:~$ cat ~/-    
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
bandit1@melinda:~$ cat <-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
Password: *CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9*
