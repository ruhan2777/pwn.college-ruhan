# Challenge Name
Mixing globs

## My solve
**Flag:** `pwn.college{gqSZnsLsHcyE9JoIf0-ksaiy6Dp.QX1IDO0wyN2kjNzEzW}`

```bash
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *in*
Error: you did not use a square bracket glob...
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *[i]*
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
amazing beautiful challenging delightful educational fantastic incredible jovial kind laughing magical nice optimistic pwning radiant splendid thrilling uplifting victorious xenial
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{gqSZnsLsHcyE9JoIf0-ksaiy6Dp.QX1IDO0wyN2kjNzEzW}
hacker@globbing~mixing-globs:/challenge/files$
```
## Incorrect tangents I went on
None

## What I learned
Learned how to use different globes in a single argument

## References 
No outside reference used
