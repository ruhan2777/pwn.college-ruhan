# Challenge Name
Catting Practice

## My solve
**Flag:** `pwn.college{s7-91kmpk-x7_eqx9HidcKm6hK1.QXwITO0wyN2kjNzEzW}`

```bash
Connected!
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /lib/x86_64-linux-gnu/ldscripts/flag. Go cat it out **without**
cding into that directory!
hacker@commands~more-catting-practice:~$ cat /lib/x86_64-linux-gnu/ldsscripts/flag
cat: /lib/x86_64-linux-gnu/ldsscripts/flag: No such file or directory
hacker@commands~more-catting-practice:~$  cat /lib/x86_64-linux-gnu/ldscripts/flag
pwn.college{s7-91kmpk-x7_eqx9HidcKm6hK1.QXwITO0wyN2kjNzEzW}
hacker@commands~more-catting-practice:~$

```
## Incorrect tangents I went on
typing error

## What I learned
Learned how to read files using cat function by giving absolute path.

## References 
No outside reference used
