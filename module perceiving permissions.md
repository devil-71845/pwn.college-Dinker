# 1. Changing File Ownership

This challenge prompted me to change the owner of a file to gain read access.

## My Solve

**Flag:** `pwn.college{g1uB6KU_7g9gWSksWmTkIS2QFmO.QXxEjN0wiM2gjNzEzW}`

I couldn't read the `/flag` file because it was owned by root. I used the `chown hacker /flag` command to change the file's owner to my user. After that, I was able to read the file with `cat`.

```
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{g1uB6KU_7g9gWSksWmTkIS2QFmO.QXxEjN0wiM2gjNzEzW}

```

## What I Learned

I learnt that the `chown` command is used to change the ownership of a file, which can affect who has permission to access it.

## References

The problem statement provided was the reference used.

```
Every file in Linux is owned by a user on the system.
...
Interestingly, we can change the ownership of files!
This is done via the chown (change owner) command:

chown [username] [file]

Typically, chown can only be invoked by the root user.
...
In this level, we will practice changing the owner of the /flag file to the hacker user, and then read the flag.
For this challenge only, I made it so that you can use chown to your heart's content as the hacker user...
```

# 2. Groups and Files

This challenge prompted me to change the group ownership of a file to gain read access.

## My Solve

**Flag:** `pwn.college{cAQXOayVknnGTDZE1XqWZda8Jyg.QXxcjM1wiM2gjNzEzW}`

The `/flag` was only readable by its group `root`. I used `chgrp hacker /flag` to change the group owner to `hacker` as my user is in the group `hacker`, I then read the file with `cat`.

```
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ ls -l /
total 64
lrwxrwxrwx    1 root root      7 Apr  4  2025 bin -> usr/bin
drwxr-xr-x    2 root root   4096 Apr 15  2020 boot
drwxr-xr-x    1 root root   4096 Oct 10 12:33 challenge
drwxr-xr-x    6 root root    380 Oct 10 12:33 dev
drwxr-xr-x    1 root root   4096 Oct 10 12:33 etc
-r--r-----    1 root hacker   60 Oct 10 12:33 flag
drwxr-xr-x    1 root root   4096 Sep 26 17:24 home
lrwxrwxrwx    1 root root      7 Apr  4  2025 lib -> usr/lib
lrwxrwxrwx    1 root root      9 Apr  4  2025 lib32 -> usr/lib32
lrwxrwxrwx    1 root root      9 Apr  4  2025 lib64 -> usr/lib64
lrwxrwxrwx    1 root root     10 Apr  4  2025 libx32 -> usr/libx32
drwxr-xr-x    2 root root   4096 Apr  4  2025 media
drwxr-xr-x    2 root root   4096 Apr  4  2025 mnt
drwxr-xr-x    1 root root     16 Oct 26  2024 nix
drwxr-xr-x    1 root root   4096 Sep 26 17:24 opt
dr-xr-xr-x 2600 root root      0 Oct 10 12:33 proc
drwx------    1 root root   4096 Sep 26 17:24 root
drwxr-xr-x    1 root root   4096 Oct 10 12:33 run
lrwxrwxrwx    1 root root      8 Apr  4  2025 sbin -> usr/sbin
drwxr-xr-x    2 root root   4096 Apr  4  2025 srv
dr-xr-xr-x   13 root root      0 Sep 23 22:44 sys
drwxrwxrwt    1 root root   4096 Oct 10 12:33 tmp
drwxr-xr-x    1 root root   4096 Sep 26 17:09 usr
drwxr-xr-x    1 root root   4096 Sep 26 17:08 var
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{cAQXOayVknnGTDZE1XqWZda8Jyg.QXxcjM1wiM2gjNzEzW}

```

## What I Learned

I learnt that the `chgrp` is used to change group ownership of a specific file, which can be a way to manage file access permissions.

## References

The problem statement provided was the reference used.

```
Files have both an owning user and group.
...
Often, this access control happens via group ownership on the filesystem!
...
Luckily, group ownership can be changed with the chgrp (change group) command!
...
In this level, I have made the flag readable by whatever group owns it, but this group is currently root.
...
Change the group ownership of the flag file, and read the flag!
```

# 3. Fun with group names

This challenge prompted me to find my user's group name and use it to change a file's group ownership.

## My Solve

**Flag:** `pwn.college{0_7Gmn6TmszNj1TD0goZb17uzSz.QXycjM1wiM2gjNzEzW}`

I used the `id` command to find my group, which was `grp16404`. I then used `chgrp` to change the `/flag` file's group to `grp16404` and read it with `cat`.

```
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp30884) groups=1000(grp30884)
hacker@permissions~fun-with-groups-names:~$  chgrp grp30884 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{0_7Gmn6TmszNj1TD0goZb17uzSz.QXycjM1wiM2gjNzEzW}

```

## What I Learned

I learnt that the `id` command is used to find out the current user's group.

## References

The problem statement provided was the reference used.

```
...in this level, that is not going to work.
I'll still allow you to use chgrp, but I have randomized the name of the group that your user is in.
You will need to use the id command to figure that name out, then chgrp to victory!
```

# 4. Changing Permissions

This challenge prompted me to change a file's permissions to make it readable.
## My Solve

**Flag:** `pwn.college{MIYe9_wKhoKF4adivNT5PfCQ7g1.QXzcjM1wiM2gjNzEzW}`

The `/flag` file was not readable by my user. I used `chmod +r /flag` to add read permissions for everyone. After that, I was able to use `cat` to read the flag.

```
hacker@permissions~changing-permissions:~$ chmod +r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{MIYe9_wKhoKF4adivNT5PfCQ7g1.QXzcjM1wiM2gjNzEzW}

```
## What I Learned

I learnt that the **`chmod`** command is used to change file permissions. You can use a symbolic format to add (`+`) or remove (`-`) permissions for the **user** (`u`), **group** (`g`), **other** (`o`), or **all** (`a`). The permissions are **read** (`r`), **write** (`w`), and **execute** (`x`). 
## References

The problem statement provided was the reference used.

```
...file permissions can also be changed.
This is done with the chmod (change mode) command.
The basic usage for chmod is:

chmod [OPTIONS] MODE FILE

...chmod allows you to tweak permissions with the mode format of WHO+/-WHAT, where WHO is user/group/other and WHAT is read/write/execute.
...
In this challenge, you must change the permissions of the /flag file to read it!
```

# 5. Executable Files

This challenge prompted me to add execute permissions to a file to run it.

## My Solve

**Flag:** `pwn.college{YYRdBBK__s3LkZcb1B1zsJz6xCT.QXyEjN0wiM2gjNzEzW}`

The `/challenge/run` binary was not executable by default. I used `chmod +x /challenge/run` to add the execute permission for my user, which then allowed me to run the program and get the flag.

```
hacker@permissions~executable-files:~$ chmod +x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{YYRdBBK__s3LkZcb1B1zsJz6xCT.QXyEjN0wiM2gjNzEzW}

```

## What I Learned

I learnt that the `x` permission is required to execute a file as a program and that it can be added using `chmod +x`.

## References

The problem statement provided was the reference used.

```
When you invoke a program, such as /challenge/run, Linux will only actually execute it if you have execute-access to the program file.
...
If we remove these permissions, the execution will fail!
...
In this challenge, the /challenge/run program will give you the flag, but you must first make it executable!
```

# 6. Permission Tweaking Practice

This challenge prompted me to solve a series of permission puzzles using `chmod`.

## My Solve

**Flag:** `pwn.college{wDHvdJGuQw2O3evBeuEmQ7olbWl.QXwEjN0wiM2gjNzEzW}`

I ran the challenge which provided with 8 rounds of setting permissions tasks. Each round I used `chmod` with the correct symbolic notation to match the required permission. After completing all rounds, I could change the permission of `/flag` file, so I `chmod +r /flag` and then `cat /flag` to read the final flag.

```
hacker@permissions~permission-tweaking-practice:~$ /challenge/run
Round 1 of 8!

Current permissions of "/challenge/pwn": rw-r--r--
* the user does have read permissions
* the user does have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": rwxr-xr--
* the user does have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 754 /challenge/pwn
You set the correct permissions!
Round 2 of 8!

Current permissions of "/challenge/pwn": rwxr-xr--
* the user does have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": rwxrwxr--
* the user does have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 774 /challenge/pwn
You set the correct permissions!
Round 3 of 8!

Current permissions of "/challenge/pwn": rwxrwxr--
* the user does have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": rwxrwxrw-
* the user does have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
- the world doesn't have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 776 /challenge/pwn
You set the correct permissions!
Round 4 of 8!

Current permissions of "/challenge/pwn": rwxrwxrw-
* the user does have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r--rwxr--
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 474 /challenge/pwn
You set the correct permissions!
Round 5 of 8!

Current permissions of "/challenge/pwn": r--rwxr--
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r--rwxrwx
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 477 /challenge/pwn
You set the correct permissions!
Round 6 of 8!

Current permissions of "/challenge/pwn": r--rwxrwx
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": r----xrwx
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 417 /challenge/pwn
You set the correct permissions!
Round 7 of 8!

Current permissions of "/challenge/pwn": r----xrwx
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": -----xrwx
- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 017 /challenge/pwn
You set the correct permissions!
Round 8 of 8!

Current permissions of "/challenge/pwn": -----xrwx
- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": -----x--x
- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
* the world does have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod 011 /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!

Current permissions of "/flag": ---------
- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permission-tweaking-practice:~$ chmod +r /flag
hacker@permissions~permission-tweaking-practice:~$ cat /flag
pwn.college{wDHvdJGuQw2O3evBeuEmQ7olbWl.QXwEjN0wiM2gjNzEzW}

```
## What I Learned

I learnt to apply `chmod`'s symbolic notation to achieve specific permission states by adding and removing read, write, and execute permissions for the user, group, and others.

## References

The problem statement provided was the reference used.

```
You think you can chmod?
Let's practice!
This challenge will ask you to change the permissions of the /challenge/pwn file in specific ways a few times in a row.
If you get the permissions wrong, the game will reset and you can try again.
If you get the permissions right eight times in a row, the challenge will let you chmod /flag to make it readable for yourself :-)
Launch /challenge/run to get started!
```

# 7. Permission Setting Practice

This challenge prompted me to solve a series of permission puzzles using `chmod`'s absolute setting (`=`) and chaining features.

## My Solve

**Flag:** `pwn.college{AB9E1hzBbF9XT0-90BYSi8OeckJ.QXzETO0wiM2gjNzEzW}`

This time I had to use `chmod` with the equals sign `=` to set exact permissions, and commas to set different permissions for the user, group, and others all in one command. After completing the rounds, I made the flag readable with `chmod +r /flag` and then read it.

```
hacker@permissions~permissions-setting-practice:~$ /challenge/run
Round 1 of 8!

Current permissions of "/challenge/pwn": rw-r--r--
* the user does have read permissions
* the user does have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r--r-----
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 440 /challenge/pwn
You set the correct permissions!
Round 2 of 8!

Current permissions of "/challenge/pwn": r--r-----
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": rw-r-xr-x
* the user does have read permissions
* the user does have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
* the world does have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 655 /challenge/pwn
You set the correct permissions!
Round 3 of 8!

Current permissions of "/challenge/pwn": rw-r-xr-x
* the user does have read permissions
* the user does have write permissions
- the user doesn't have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": --x-wxrw-
- the user doesn't have read permissions
- the user doesn't have write permissions
* the user does have execute permissions
- the group doesn't have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
- the world doesn't have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 136 /challenge/pwn
You set the correct permissions!
Round 4 of 8!

Current permissions of "/challenge/pwn": --x-wxrw-
- the user doesn't have read permissions
- the user doesn't have write permissions
* the user does have execute permissions
- the group doesn't have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r----x---
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 410 /challenge/pwn
You set the correct permissions!
Round 5 of 8!

Current permissions of "/challenge/pwn": r----x---
* the user does have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r-x-wx--x
* the user does have read permissions
- the user doesn't have write permissions
* the user does have execute permissions
- the group doesn't have read permissions
* the group does have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
* the world does have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 531 /challenge/pwn
You set the correct permissions!
Round 6 of 8!

Current permissions of "/challenge/pwn": r-x-wx--x
* the user does have read permissions
- the user doesn't have write permissions
* the user does have execute permissions
- the group doesn't have read permissions
* the group does have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": --xr-x-wx
- the user doesn't have read permissions
- the user doesn't have write permissions
* the user does have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
* the world does have write permissions
* the world does have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 153 /challenge/pwn
You set the correct permissions!
Round 7 of 8!

Current permissions of "/challenge/pwn": --xr-x-wx
- the user doesn't have read permissions
- the user doesn't have write permissions
* the user does have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
* the group does have execute permissions
- the world doesn't have read permissions
* the world does have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": -wx-wxr-x
- the user doesn't have read permissions
* the user does have write permissions
* the user does have execute permissions
- the group doesn't have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
* the world does have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 335 /challenge/pwn
You set the correct permissions!
Round 8 of 8!

Current permissions of "/challenge/pwn": -wx-wxr-x
- the user doesn't have read permissions
* the user does have write permissions
* the user does have execute permissions
- the group doesn't have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
- the world doesn't have write permissions
* the world does have execute permissions

Needed permissions of "/challenge/pwn": -wxr--rwx
- the user doesn't have read permissions
* the user does have write permissions
* the user does have execute permissions
* the group does have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod 347 /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!

Current permissions of "/flag": ---------
- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions
hacker@permissions~permissions-setting-practice:~$ chmod +r /flag
hacker@permissions~permissions-setting-practice:~$ cat /flag
pwn.college{AB9E1hzBbF9XT0-90BYSi8OeckJ.QXzETO0wiM2gjNzEzW}

```

## What I Learned

I learnt that `chmod` can set exact permissions with the `=` operator, overwriting the old ones. I also learnt that you can chain multiple permission changes for user, group, and other by separating them with a comma.

## References

The problem statement provided was the reference used.

```
In addition to adding and removing permissions, as in the previous level, chmod can also simply set permissions altogether, overwriting the old ones.
This is done by using = instead of - or +.
...
You can achieve this by chaining multiple modes to chmod with ,!

chmod u=rw,g=r /challenge/pwn will set the user permissions to read and write, and the group permissions to read-only
...
This level extends the previous level by requesting more radical permission changes, which you will need = and ,-chaining to achieve.
```


# 8. The SUID Bit
This challenge prompted me to set the SUID bit on an executable to gain root privileges.

## My Solve

**Flag:** `pwn.college{AdfadB7oIVKRMtYO5CMj7isu1TW.QXzEjN0wiM2gjNzEzW}`

I used `chmod u+s` to set the SUID bit on the `/challenge/getroot` program. When I ran it, the program executed as the owner (root) because of the SUID bit, which gave me a root shell. From there, I was able to read the flag with `cat /flag`.

```
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{AdfadB7oIVKRMtYO5CMj7isu1TW.QXzEjN0wiM2gjNzEzW}

```

## What I Learned

I learnt that the SUID permission bit (`s`) allows a program to run with the privileges of its owner, not the user who runs it. It can be set with `chmod u+s`.

## References

The problem statement provided was the reference used.

```
...the "Set User ID" (SUID) permissions bit allows the user to run a program as the owner of that program's file.
...
The s part in place of the executable bit means that the program is executable with SUID.
...
As the owner of a file, you can set a file's SUID bit by using chmod:

chmod u+s [program]
...
Now, we are going to let you add the SUID bit to the /challenge/getroot program in order to spawn a root shell for you to cat the flag yourself!
```
