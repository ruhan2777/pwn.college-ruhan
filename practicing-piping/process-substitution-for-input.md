# Challenge Name
Process Substitution For Input

## My solve
**Flag:** `pwn.college{Y8Z5LuxgyJzpcw_LmUStnNch5R7.0lNwMDOxwyN2kjNzEzW}`

```bash
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
63a64
84a85
> pwn.college{Y8Z5LuxgyJzpcw_LmUStnNch5R7.0lNwMDOxwyN2kjNzEzW}
bash: 63a64: command not found
hacker@piping~process-substitution-for-input:~$
```
## Incorrect tangents I went on
None

## What I learned
Learned how you can directly use a command without first saving into the files mainly when the command takes an argument

## References 
No outside reference used
