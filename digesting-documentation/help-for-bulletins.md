# Challenge Name
Help For Builtins

## My solve
**Flag:** `pwn.college{AHiwzGlukzykLIjRl2Yq6MGZVMn.QX0ETO0wyN2kjNzEzW}`

```bash
Connected!
hacker@man~help-for-builtins:~$ client_loop: send disconnect: Broken pipe
darsh@DESKTOP-19U3OG4:~$ ssh -i key hacker@dojo.pwn.college
Connected!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "AHiwzGlu".
hacker@man~help-for-builtins:~$ challenge --secret AHiwzGlu
Correct! Here is your flag!
pwn.college{AHiwzGlukzykLIjRl2Yq6MGZVMn.QX0ETO0wyN2kjNzEzW}

hacker@man~help-for-builtins:~$

```
## Incorrect tangents I went on
None

## What I learned
Learned how to use help command to get help for the builtins functions

## References 
No outside reference used
