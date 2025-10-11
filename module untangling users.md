# 1. Becoming root with `su`

This challenge prompted me to gain root access using the `su` command and a password.

## My Solve

**Flag:** `pwn.college{o30HDO3q4Nkep3yfdjp2o3egLv-.QX1UDN1wiM2gjNzEzW}`

I used the `su` command and, when prompted, entered the password `hack-the-planet`. This gave me a root shell, and I then used `cat /flag` to read the flag.

```
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{o30HDO3q4Nkep3yfdjp2o3egLv-.QX1UDN1wiM2gjNzEzW}

```

## What I Learned

I learnt that the `su` command can be used to switch to the root user by providing the root password.

## References

The problem statement provided was the reference used.

```
It's not just hackers that need to become root.
...
Becoming root is a fairly common action that Linux users take, and there are two utilities that exist for this purpose: su and sudo.
In this challenge, we will cover the older one, su (the substitute user command).
...
before allowing the user to elevate privileges to root, it checks to make sure that the user knows the root password...
...
That password is hack-the-planet, and you must provide it to su to become root!
```

# 2. Other users with `su`
This challenge prompted me to switch to a different user account using `su`.

## My Solve

**Flag:** `pwn.college{IqxifHCMUoAMezkDBiEwZuh0ayG.QX2UDN1wiM2gjNzEzW}`

I used `su zardus` to switch the current user to `zardus`. Then I entered the password `dont-hack-me` and then ran the `/challenge/run` program to get the flag.

```
hacker@users~other-users-with-su:~$ su zardus
Password: 
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{IqxifHCMUoAMezkDBiEwZuh0ayG.QX2UDN1wiM2gjNzEzW}

```

## What I Learned

I learnt that `su` can be used to switch to any user by providing the target username in the argument.

## References

The problem statement provided was the reference used.

```
With no arguments, su will start a root shell (after authenticating with root's password).
However, you can also give a username as an argument to switch to that user instead of root.
For example:

hacker@dojo:~$ su some-user
Password: 
some-user@dojo:~$

In this level, you must switch to the zardus user and then run /challenge/run.
Zardus' password is dont-hack-me.
```

# 3. Cracking passwords

This challenge prompted me to use the `su` command to run/access a file by entering a secret password after running through some directory.
## My solve	

**Flag:** `pwn.college{0DFeSyn4EgdUcZW8V4W71SlOzeW.QX3UDN1wiM2gjNzEzW}`



```
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:14 0% 2/3 0g/s 295.3p/s 295.3c/s 295.3C/s billy1..december
aardvark         (zardus)
1g 0:00:00:19 1% 2/3 0.05141g/s 299.3p/s 299.3c/s 299.3C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session aborted
hacker@users~cracking-passwords:~$ john --show /challenge/shadow-leak
hacker:NO PASSWORD:20357:0:99999:7:::
zardus:aardvark:20372:0:99999:7:::

2 password hashes cracked, 0 left
hacker@users~cracking-passwords:~$ su zardus
Password:
su: Authentication failure
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{0DFeSyn4EgdUcZW8V4W71SlOzeW.QX3UDN1wiM2gjNzEzW}

```
## What I Learned

I learnt that `sudo` is used to run a single command with root privileges, which is a common way to perform administrative tasks.

## References

The problem statement provided was the reference used.

```
...in recent decades, the world has moved from 
administration via su to administration via sudo...
...
In this challenge the secret password to access the secret files is aardvark...


# 4. Using `sudo`

This challenge prompted me to use the `sudo` command to run a command with root privileges.
## My Solve

**Flag:** `pwn.college{oqq5rxMC0tXEkJs6jddW-rXBqu5.QX4UDN1wiM2gjNzEzW}`

I first tried to read the flag with `cat` but got permission denied error. Then I ran the same command with `sudo` to execute as root which gave me the permission to read the file.

```
hacker@users~using-sudo:~$ cat /flag
cat: /flag: Permission denied
hacker@users~using-sudo:~$ sudo cat /flag
pwn.college{oqq5rxMC0tXEkJs6jddW-rXBqu5.QX4UDN1wiM2gjNzEzW}

```

## What I Learned

I learnt that `sudo` is used to run a single command with root privileges, which is a common way to perform administrative tasks.

## References

The problem statement provided was the reference used.

```
...in recent decades, the world has moved from 
administration via su to administration via sudo...
...
Unlike su, which defaults to launching a shell as a specified user, sudo defaults to running a command as root:

hacker@dojo:~$ whoami
hacker
hacker@dojo:~$ sudo whoami
root
hacker@dojo:~$

In this level, we will give you sudo access, and you will use it to read the flag.
```
