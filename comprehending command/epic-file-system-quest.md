# Challenge Name
An Epic Filesystem Quest

## My solve
**Flag:** `pwn.college{YBwiKuDR47pJaHHVpB8P4qeszs8.QX5IDO0wyN2kjNzEzW}`

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
MEMO  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin   challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat MEMO
Tubular find!
The next clue is in: /usr/lib/python3/dist-packages/sympy/geometry/tests
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/sympy/geometry/tests
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/geometry/tests$ ls
BLUEPRINT    __pycache__    test_ellipse.py  test_geometrysets.py  test_parabola.py  test_point.py    test_util.py
__init__.py  test_curve.py  test_entity.py   test_line.py          test_plane.py     test_polygon.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/geometry/tests$ cat BLUEPRINT
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/zipp

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/geometry/tests$ cd /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/zipp
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/zipp$ ls
SNIPPET  __init__.py  __pycache__  compat  glob.py
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/zipp$ cat SNIPPET
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/angr/knowledge_plugins/variables/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/zipp$ cd /usr/local/lib/python3.8/dist-packages/angr/knowledge_plugins/variables/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/angr/knowledge_plugins/variables/__pycache__$ ls -a
.  ..  .NUGGET  __init__.cpython-38.pyc  variable_access.cpython-38.pyc  variable_manager.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/angr/knowledge_plugins/variables/__pycache__$ cat .NUGGET
Tubular find!
The next clue is in: /opt/linux/linux-5.4/include/config/inline/read/unlock
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/angr/knowledge_plugins/variables/__pycache__$ cd /opt/linux/linux-5.4/include/config/inline/read/unlock
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ ls
LEAD  irq.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ cat LEAD
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/sound/soc/ux500

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ ls /opt/linux/linux-5.4/sound/soc/ux500 -a
.   .GIST    Makefile  mop500_ab8500.c  ux500_msp_dai.c  ux500_msp_i2s.c  ux500_pcm.c
..  Kconfig  mop500.c  mop500_ab8500.h  ux500_msp_dai.h  ux500_msp_i2s.h  ux500_pcm.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ cat /opt/linux/linux-5.4/sound/soc/ux500/.GIST
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/include/config/mutex
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ ls /opt/linux/linux-5.4/include/config/mutex
NOTE  spin
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ cat /opt/linux/linux-5.4/include/config/mutex/NOTE
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/arm/mach-aspeed

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/inline/read/unlock$ cd /opt/linux/linux-5.4/arch/arm/mach-aspeed
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-aspeed$ ls
DOSSIER  Kconfig  Makefile  platsmp.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-aspeed$ cat DOSSIER
Yahaha, you found me!
The next clue is in: /usr/lib/python3/dist-packages/sage/arith/__pycache__

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-aspeed$ ls /usr/lib/python3/dist-packages/sage/arith/__pycache__
DISPATCH-TRAPPED  __init__.cpython-38.pyc  all.cpython-38.pyc  misc.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-aspeed$ cat /usr/lib/python3/dist-packages/sage/arith/__pycache__/DISPATCH-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{YBwiKuDR47pJaHHVpB8P4qeszs8.QX5IDO0wyN2kjNzEzW}
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-aspeed$
```
## Incorrect tangents I went on
None

## What I learned
Applied the knowledge of ls, cd, cat commands

## References 
No outside reference used
