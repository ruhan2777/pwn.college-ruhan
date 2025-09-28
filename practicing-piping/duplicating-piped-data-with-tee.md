# Challenge Name
Duplicating Piped Output Using Tee

## My solve
**Flag:** `pwn.college{8fi0Qf2gDLInIjDRID8CdM4-gs1.QXxITO0wyN2kjNzEzW}`

```bash
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pwn_out | /challenge/college
Processing...
WARNING: you are overwriting file pwn_out with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn_out
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "8fi0Qf2g"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 8fi0Qf2g | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{8fi0Qf2gDLInIjDRID8CdM4-gs1.QXxITO0wyN2kjNzEzW}
hacker@piping~duplicating-piped-data-with-tee:~$
```
## Incorrect tangents I went on
None

## What I learned
Learned how to duplicate the output of a particular output in a file using the tee function

## References 
No outside reference used
