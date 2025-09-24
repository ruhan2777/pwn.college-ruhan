# Challenge Name
Hidden Files

## My solve
**Flag:** `pwn.college{486LRSGEtnlSWEO2q8uzDR7QPsE.QXwUDO0wyN2kjNzEzW}

```bash
Connected!
hacker@commands~hidden-files:~$ ls / -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-32532132757865  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:~$  cat/.flag-32532132757865
bash: cat/.flag-32532132757865: No such file or directory
hacker@commands~hidden-files:~$ cat /.flag-32532132757865
pwn.college{486LRSGEtnlSWEO2q8uzDR7QPsE.QXwUDO0wyN2kjNzEzW}
hacker@commands~hidden-files:~$

```
## Incorrect tangents I went on
typing error

## What I learned
Learned how to show the hidden files that start with '.'

## References 
No outside reference used
