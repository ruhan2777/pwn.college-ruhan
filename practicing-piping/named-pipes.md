# Challenge Name
Named Pipe

## My solve
**Flag:** `pwn.college{wWG_hnpTCg9paOD8XSNSQbyZUJn.01MzMDOxwyN2kjNzEzW}`

```bash
Connected!
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo | cat /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{wWG_hnpTCg9paOD8XSNSQbyZUJn.01MzMDOxwyN2kjNzEzW}
hacker@piping~named-pipes:~$
```
## Incorrect tangents I went on
None

## What I learned
Learned how to make a pipe file giving a personalised name using the mkfifo command

## References 
No outside reference used
