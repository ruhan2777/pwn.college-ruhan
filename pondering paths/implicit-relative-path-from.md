# Challenge Name
Implicit Relative Path From

## My solve
**Flag:** `pwn.college{Iat4FGmHMDNkiQtqJPEnmfy-yv8.QX5QTN0wyN2kjNzEzW}`

```bash
Connected!
hacker@paths~implicit-relative-paths-from-:~$ cd /challenge
hacker@paths~implicit-relative-paths-from-:/challenge$ ./run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:/challenge$ cd /
hacker@paths~implicit-relative-paths-from-:/$ ./run
bash: ./run: Is a directory
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Iat4FGmHMDNkiQtqJPEnmfy-yv8.QX5QTN0wyN2kjNzEzW}
hacker@paths~implicit-relative-paths-from-:/$


```
## Incorrect tangents I went on
Put aboslute path instead of the relative path (confusion in the syntax)

## What I learned
Learned how to access a program using relative path using the cwd

## References 
No outside reference used
