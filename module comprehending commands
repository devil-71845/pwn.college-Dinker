# 1. cat: not the pet, but the command!
The challenge prompted me to invoke cat command on the bash script, 
The command `cat` was introduced.

## My Solve
**Flag:** `pwn.college{QbtI0-huXkbm6jWm3mL0fQKk3Z2.QXxcTN0wiM2gjNzEzW}`

In the problem statement, it was provided that, Finally, if you give no arguments at all, cat will read from the terminal input and output it. We'll explore that in later challenges...

In this challenge, I will copy the flag to the flag file in your home directory (where your shell starts). Go read it with cat!
```
hacker@commands~cat-not-the-pet-but-the-command:~$ cat flag
pwn.college{QbtI0-huXkbm6jWm3mL0fQKk3Z2.QXxcTN0wiM2gjNzEzW}
hacker@commands~cat-not-the-pet-but-the-command:~$

```

## What I learned
I learnt to invoke cat command,
I learnt to invoke `cat`,
The problem required me to run the command 'cat', which displayed me the flag.

## References
The problem statement was the reference used.
```
Here, the user executed the cat command, which simply gives the file (flag) to the terminal.
```
# 2. catting absolute paths
The challenge prompted me to invoke cat command on the script in /flag file, 
The command `cat` was introduced.

## My Solve
**Flag:** `pwn.college{0sHWRKHrs3-czg3MhDejekAhZ4s.QX5ETO0wiM2gjNzEzW}`

In the problem statement, it was provided that, Finally, if you give no arguments at all, cat will read from the terminal input and output it. We'll explore that in later challenges...

In this challenge, I will copy the flag to the flag file in your home directory (where your shell starts). Go read it with cat!

In this directory, I will not copy it to your home directory, but I will make it readable. You can read it with cat at its absolute path: /flag.

/flag is where the flag always lives in pwn.college, but unlike in this challenge, you typically can't access that file directly.
```
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{0sHWRKHrs3-czg3MhDejekAhZ4s.QX5ETO0wiM2gjNzEzW}
hacker@commands~catting-absolute-paths:~$


```

## What I learned
I learnt to invoke cat command,
I learnt to invoke `cat`,
The problem required me to run the command 'cat', which displayed me the flag.

## References
The problem statement was the reference used.
```
Here, the user executed the cat command, which simply gives the file (flag) to the terminal.
```

# 3. more catting practice
The challenge prompted me to invoke cat command on the script in /lib/systemd/system/flag file, 
The command `cat` was introduced.

## My Solve
**Flag:** `pwn.college{YldPCA4gWAi-uJqyliqs1fGDMgT.QXwITO0wiM2gjNzEzW}`

In the problem statement,You can specify all sorts of paths as arguments to commands, and we'll practice some more with cat. In this level, I'll put the flag in some crazy directory, and I will not allow you to change directories with cd, so no cat flag for you. You must retrieve the flag by absolute path, wherever it is.

we have to retrieve the flag file from /lib/systemd/system/flag without using cd. 

/flag is where the flag always lives in pwn.college, but unlike in this challenge, you typically can't access that file directly.
```
hacker@commands~more-catting-practice:~$ cat /lib/systemd/system/flag
pwn.college{YldPCA4gWAi-uJqyliqs1fGDMgT.QXwITO0wiM2gjNzEzW}
hacker@commands~more-catting-practice:~$


```

## What I learned
I learnt to invoke cat command,
I learnt to invoke `cat`,
The problem required me to run the command 'cat', which displayed me the flag.

## References
The problem statement was the reference used.
```
Here, the user executed the cat command, which simply gives the file (flag) to the terminal.
```

# 4. grepping for a needle in a haystack
The challenge prompted me to invoke grep command on the bash script /challenge/data.txt file , 
The command `grep` was introduced.

## My Solve
**Flag:** `pwn.college{cp8i5RdH_6_q-X_9tZ6mdz24L2N.QX3EDO0wiM2gjNzEzW}`

In the problem statement,Invoked like this, grep will search the file for lines of text containing SEARCH_STRING and print them to the console.

If we invoke grep to a file to be searched in specified directory.It will search all files with given file name in that directory.

In this challenge, I've put a hundred thousand lines of text into the /challenge/data.txt file. grep it for the flag!
```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn /challenge/data.txt
pwns
pwned
pwning
pwn.college{cp8i5RdH_6_q-X_9tZ6mdz24L2N.QX3EDO0wiM2gjNzEzW}
pwn
hacker@commands~grepping-for-a-needle-in-a-haystack:~$

```
## What I learned
I learnt to invoke grep command,
I learnt to invoke `grep`,
The problem required me to run the command 'grep', which displayed me the flag.

## References
The problem statement was the reference used.
```
Here, the hint to find file is: The flag always starts with the text pwn.college.
```
# 5. comparing files
The challenge prompted me to invoke diff command on the bash script to find difference between 2 files, 
The command `diff` was introduced.

## My Solve
**Flag:** `pwn.college{ow6x774UlAriIgbTKO8-A9fBVy9.01MwMDOxwiM2gjNzEzW}`

In the problem statement, diff compares two files line by line and shows you exactly what's different between them.

for your challenge! There are two files in /challenge:

/challenge/decoys_only.txt contains 100 fake flags
/challenge/decoys_and_real.txt contains all 100 fake flags plus the one real flag
Use diff to find what's different between these files and get your flag!
```
hacker@commands~comparing-files:~$ cd /challenge
hacker@commands~comparing-files:/challenge$ diff decoys_only.txt decoys_and_real.txt
87a88
> pwn.college{ow6x774UlAriIgbTKO8-A9fBVy9.01MwMDOxwiM2gjNzEzW}
hacker@commands~comparing-files:/challenge$


```

## What I learned
I learnt to invoke  diff command,
I learnt to invoke `diff`,
The problem required me to run the command 'diff', which displayed me the comparison of the 2 files to get the flag.

## References
The problem statement was the reference used.
```
Here, the user executed the diff command, which simply gives the file (flag) to the terminal.by showing difference between two files.
```

# 6. listing files
The challenge prompted me to invoke ls command on the bash script /challenge/ , 
The command `ls` was introduced.

## My Solve
**Flag:** `pwn.college{UBKyxDHT2rGKfr4hktnYn1xvwkV.QX4IDO0wiM2gjNzEzW}`

In the problem statement,Invoked like this, ls will display the files present in the given directory and print them to the console.

If we invoke ls to a file to be searched in specified directory.It will search all files with given directory name.

```
hacker@commands~listing-files:~$ ls /challenge
18863-renamed-run-7955  DESCRIPTION.md
hacker@commands~listing-files:~$ cd /challenge
hacker@commands~listing-files:/challenge$ ls
18863-renamed-run-7955  DESCRIPTION.md
hacker@commands~listing-files:/challenge$ cat 18863-renamed-run-7955
#!/opt/pwn.college/bash

echo "Yahaha, you found me! Here is your flag:"
cat /flag
hacker@commands~listing-files:/challenge$ ./18863-renamed-run-7955
Yahaha, you found me! Here is your flag:
pwn.college{UBKyxDHT2rGKfr4hktnYn1xvwkV.QX4IDO0wiM2gjNzEzW}
hacker@commands~listing-files:/challenge$


```
## What I learned
I learnt to invoke ls command,
I learnt to invoke `ls`,
The problem required me to run the command 'ls', which displayes all the files.

## References
The problem statement was the reference used.
```
But directories can have lots of files (and other directories) inside them, and we won't always be here to tell you their names. You'll need to learn to list their contents using the ls command! 
In this challenge, They've named /challenge/run with some random name! List the files in /challenge to find it.
ls will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided.
```

# 7. touching files
The challenge prompted me to invoke touch command on the script to create files, 
The command `touch` was introduced.

## My Solve
**Flag:** `pwn.college{IKuqYw-iPuKtkMCRAIdsw-iKSCZ.QXwMDO0wiM2gjNzEzW}`

In the problem statement, touch creates two files and we need to run /challenge/run to get the flag.

for your challenge! create two files and run /challenge/run to get flag:

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ cd
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{IKuqYw-iPuKtkMCRAIdsw-iKSCZ.QXwMDO0wiM2gjNzEzW}
hacker@commands~touching-files:~$

```

## What I learned
I learnt to invoke touch command,
I learnt to invoke `touch`,
The problem required me to run the command 'touch', which creates 2 files.

## Reference
The problem statement was the reference used.
```
It's that simple! In this level, please create two files: /tmp/pwn and /tmp/college, and run /challenge/run to get your flag!
```


# 8. removing files
The challenge prompted me to invoke rm command on the script to remove files, 
The command `rm` was introduced.

## My Solve
**Flag:** `pwn.college{cP-9AssA0efoFk_NUIQ68IUvBQ_.QX2kDM1wiM2gjNzEzW}`

In the problem statement, rm removes files and we need to run /challenge/check to get the flag.

for your challenge! remove file and run /challenge/check to get flag:

```
hacker@commands~removing-files:~$ ls
Desktop  a  delete_me  t.txt
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{cP-9AssA0efoFk_NUIQ68IUvBQ_.QX2kDM1wiM2gjNzEzW}
hacker@commands~removing-files:~$

```

## What I learned
I learnt to invoke rm command,
I learnt to invoke `rm`,
The problem required me to run the command 'rm', which removes a file.

## Reference
The problem statement was the reference used.
```
This challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check, which will make sure you've deleted it and then give you the flag!
```

# 9. moving files
The challenge prompted me to invoke mv command on the script to move files, 
The command `mv` was introduced.

## My Solve
**Flag:** `pwn.college{cP-9AssA0efoFk_NUIQ68IUvBQ_.QX2kDM1wiM2gjNzEzW}`

In the problem statement, mv moves files and we need to run /challenge/check to get the flag.

for your challenge! move /flag into /tmp/hack-the-planet and run /challenge/check to get flag:

```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{cvwCRqxxP6Dk1w3PQJ_OAm1Ig8R.0VOxEzNxwiM2gjNzEzW}

hacker@commands~moving-files:~$


```

## What I learned
I learnt to invoke mv command,
I learnt to invoke `mv`,
The problem required me to run the command 'mv', which moves a file.

## Reference
The problem statement was the reference used.
```
This challenge wants you to move the /flag file into /tmp/hack-the-planet (do it)! When you're done, run /challenge/check, which will check things out and give the flag to you.
```

# 10. hidden files
The challenge prompted me to invoke ls -a command on the script to view secret files, 
The command `ls -a` was introduced.

## My Solve
**Flag:** `pwn.college{MVzYe1bSrEz3drGkKS799LWtR83.QXwUDO0wiM2gjNzEzW}`

In the problem statement, ls -a reads secret files and we need to find the flag hidden as a dot-prepended file in /..

```
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-28802343616488  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-28802343616488
pwn.college{MVzYe1bSrEz3drGkKS799LWtR83.QXwUDO0wiM2gjNzEzW}
hacker@commands~hidden-files:/$


```

## What I learned
I learnt to invoke ls -a command,
I learnt to invoke `ls -a`,
The problem required me to run the command 'ls -a', which shows a hidden file.

## Reference
The problem statement was the reference used.
```
Interestingly, ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag.

Now, it's your turn! Go find the flag, hidden as a dot-prepended file in /.
```

# 11. An epic filesystem quest
The challenge prompted me to invoke ls -a command on the script to view secret files, 
The command `ls -a` was introduced.

## My Solve
**Flag:** `pwn.college{ACNjCttBJOwoK1X1YgcKayQTuID.QX5IDO0wiM2gjNzEzW}`

In this challenge, I have hidden the flag! Here, you will use ls and cat to follow my breadcrumbs and find it! Here's how it'll work:

Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!
Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!

```
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
..  REVELATION  boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~an-epic-filesystem-quest:/$ cat REVELATION
Tubular find!
The next clue is in: /opt/linux/linux-5.4/sound/soc/bcm
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/linux/linux-5.4/sound/soc/bcm
cat: /opt/linux/linux-5.4/sound/soc/bcm: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.4/sound/soc/bcm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/sound/soc/bcm$ ls -a
.  ..  BLUEPRINT  Kconfig  Makefile  bcm2835-i2s.c  cygnus-pcm.c  cygnus-ssp.c  cygnus-ssp.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/sound/soc/bcm$ cat BLUEPRINT
Yahaha, you found me!
The next clue is in: /usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Symbols/Regular

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/sound/soc/bcm$ cd  /usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Symbols/Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Symbols/Regular$ ls -a
.  ..  Main.js  POINTER
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Symbols/Regular$ cat POINTER
Lucky listing!
The next clue is in: /usr/share/doc/libnspr4
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Symbols/Regular$ cd  /usr/share/doc/libnspr4
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libnspr4$ ls -a
.  ..  INSIGHT  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libnspr4$ cat INSIGHT
Great sleuthing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/jaraco.text-3.12.1.dist-info
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libnspr4$ cd /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/jaraco.text-3.12.1.dist-info
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/jaraco.text-3.12.1.dist-info$ ls -a
.  ..  INSTALLER  LICENSE  METADATA  RECORD  REQUESTED  SPOILER  WHEEL  top_level.txt
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/jaraco.text-3.12.1.dist-info$ cat SPOILER
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/jaraco.text-3.12.1.dist-info$ cd /usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__$ ls -a
.   .TIP                     fcfg.cpython-38.pyc                feature_structure.cpython-38.pyc
..  __init__.cpython-38.pyc  feature_production.cpython-38.pyc  state.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__$ cat .TIP
Tubular find!
The next clue is in: /usr/lib/python2.7/dist-packages

hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__$ ls /usr/lib/python2.7/dist-packages
README-TRAPPED  lsb_release.py
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__$ cat /usr/lib/python2.7/dist-packages/README-TRAPPED
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/nvkm/engine/sec2

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/pyformlang/fcfg/__pycache__$ cd /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/nvkm/engine/sec2
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/nouveau/nvkm/engine/sec2$ ls -a
.  ..  Kbuild  MESSAGE  base.c  gp102.c  priv.h  tu102.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/nouveau/nvkm/engine/sec2$ cat MESSAGE
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/Documentation/devicetree/bindings/security/tpm

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/nouveau/nvkm/engine/sec2$ cd /opt/linux/linux-5.4/Documentation/devicetree/bindings/security/tpm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/devicetree/bindings/security/tpm$ ls -a
.  ..  .TEASER  ibmvtpm.txt  st33zp24-i2c.txt  st33zp24-spi.txt  tpm-i2c.txt  tpm_tis_mmio.txt  tpm_tis_spi.txt
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/devicetree/bindings/security/tpm$ cat .TEASER
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{ACNjCttBJOwoK1X1YgcKayQTuID.QX5IDO0wiM2gjNzEzW}
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/devicetree/bindings/security/tpm$

```

## What I learned
I learnt to invoke multiple 'ls -a' and 'ls' command,
I learnt to invoke `ls -a`,
The problem required me to run the command 'ls -a', which shows a hidden file.
I learnt to discover hidden files and go through the hints at my high level possible

## Reference
The problem statement was the reference used.
```
Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!
Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!
```

# 12. making directories
The challenge prompted me to invoke mkdir command on the script to make new directories, 
The command `mkdir and rmdir` was introduced.

## My Solve
**Flag:** `pwn.college{ADP-ExCefzFQo66tYoW0yZoLJ9D.QXxMDO0wiM2gjNzEzW}`

In the problem statement, We can create files. How about directories? You make directories using the mkdir command.

```
hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:/tmp$ mkdir pwn
hacker@commands~making-directories:/tmp$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ cd
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{ADP-ExCefzFQo66tYoW0yZoLJ9D.QXxMDO0wiM2gjNzEzW}
hacker@commands~making-directories:~$

```

## What I learned
I learnt to invoke mkdir command,
I learnt to invoke `mkdir`,
The problem required me to run the command 'touch' and 'mkdir', which creates a file and makes a new directory.

## Reference
The problem statement was the reference used.
```
Create a /tmp/pwn directory and make a college file in it! Then run /challenge/run, which will check your solution and give you the flag!```






