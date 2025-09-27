# Challenge Name
Redirecting Output

## My solve
**Flag:** `pwn.college{gvUIZ-oQ3rcIFfYwyeeOdEr2pXV.QX1YTN0wyN2kjNzEzW}`

```bash
Connected!
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{gvUIZ-oQ3rcIFfYwyeeOdEr2pXV.QX1YTN0wyN2kjNzEzW}

hacker@piping~redirecting-more-output:~$
```
## Incorrect tangents I went on
None

## What I learned
Learned how to redirect any output from a command to a file

## References 
No outside reference used
