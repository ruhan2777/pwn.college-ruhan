# Challenge Name
Position Elsewhere

## My solve
**Flag:** `pwn.college{s-chfZldKyp541G2tphC0UalItH.QX3QTN0wyN2kjNzEzW}`

```bash
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /etc/apt/sources.list.d directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /etc/apt/sources.list.d
hacker@paths~position-elsewhere:/etc/apt/sources.list.d$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{s-chfZldKyp541G2tphC0UalItH.QX3QTN0wyN2kjNzEzW}
hacker@paths~position-elsewhere:/etc/apt/sources.list.d$

```
## Incorrect tangents I went on
None

## What I learned
Learned how to access a program using absolute path that is in a different direcctory

## References 
No outside reference used
