# 1. The Root
The challenge prompted me to invoke my root directory and, 


## My Solve
**Flag:** `pwn.college{Aqvj-RDOXX1Dgacg1yGRhmEjTGc.QX4cTO0wiM2gjNzEzW}`

In the problem statement,You can invoke a program by providing its path on the command line. In this case, you'll be giving the exact path, starting from /, so the path would be /pwn. This style of path, one that starts with the root directory, is referred to as an "absolute path"
```
hacker@paths~the-root:~$ cd /home
hacker@paths~the-root:/home$ /pwn
BOOM!!!
Here is your flag:
pwn.college{Aqvj-RDOXX1Dgacg1yGRhmEjTGc.QX4cTO0wiM2gjNzEzW}
hacker@paths~the-root:/home$
```

## What I learned
I learnt to invoke root directory,
I learnt to invoke `a file inside a directory`,
The problem required me to run the command 'cd /home', which lead me to the home directory.

## References
The problem statement was the reference used.
```
As they given the filesystem starts at /. Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags. In this level, they have added a program right in /, called pwn, that will give you the flag. All we need to do for this level is to invoke this program!
```


# 2. Programs and absolute paths 
The challenge prompted me to use arguments with commands,
The command "echo" was introduced.

## My solve
**Flag:** `pwn.college{AdzarobtsQocXDpzjLEvn0BiCkw.QX1QTN0wiM2gjNzEzW}`

I was provided in the problem statement that using the `hackers` argument with the `hello` command would prompt the flag.

```
hacker@paths~program-and-absolute-paths:~$ cd /run
hacker@paths~program-and-absolute-paths:/run$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{AdzarobtsQocXDpzjLEvn0BiCkw.QX1QTN0wiM2gjNzEzW}
hacker@paths~program-and-absolute-paths:/run$

```

## What I learned
I learnt how to use path function to locate file commands,
I learnt what is the use of absolute path,`
The problem required to me invoke the `Absolute paths` command with a specified argument to find the flag.

## References
The problem statement provided was used as the reference
```
Let's explore a slightly more complicated path! Except for in the previous level, challenges in pwn.college are in the challenge directory and the challenge directory is, in turn, right in the root directory (/). The path to the challenge directory is, thus, /challenge. The name of the challenge program in this level is run, and it lives in the /challenge directory. Thus, the path to the run challenge program is /challenge/run.

In this challenge, to get the flag, you must run the challenge program using absolute path.
```


# 3. Position Thy Self
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{Uq9XiuLMAifEKbfCGMKXylI1QqU.QX2QTN0wiM2gjNzEzW}`

```
hacker@paths~position-thy-self:~$ cd /challenge
hacker@paths~position-thy-self:/challenge$ ./run
Incorrect...
You are not currently in the /etc/apt/sources.list.d directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:/challenge$ cd /etc/apt/sources.list.d
hacker@paths~position-thy-self:/etc/apt/sources.list.d$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Uq9XiuLMAifEKbfCGMKXylI1QqU.QX2QTN0wiM2gjNzEzW}
hacker@paths~position-thy-self:/etc/apt/sources.list.d$
```

The flag was revealed after changing `directories` once.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,

## References
I just used the problem statement as my reference
```
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now we can see what the ~ was in the prompt! It shows the current path that your shell is located at.

This challenge will requires us to execute the /challenge/run program from a specific path (which it will tell you). we'll need to cd to that directory before rerunning the challenge program.

```

# 4. Position Elsewhere
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{wpViTgsnF42_AkCToEzJNmko13o.QX3QTN0wiM2gjNzEzW}`

```
hacker@paths~position-elsewhere:~$ cd /challenge
hacker@paths~position-elsewhere:/challenge$ ./run
Incorrect...
You are not currently in the /usr/include directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:/challenge$ cd /usr/include
hacker@paths~position-elsewhere:/usr/include$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wpViTgsnF42_AkCToEzJNmko13o.QX3QTN0wiM2gjNzEzW}
hacker@paths~position-elsewhere:/usr/include$
```

The flag was revealed after changing `directories` once.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,

## References
I just used the problem statement as my reference
```
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now we can see what the ~ was in the prompt! It shows the current path that your shell is located at.

This challenge will requires us to execute the /challenge/run program from a specific path (which it will tell you). we'll need to cd to that directory before rerunning the challenge program.

```



# 5. Position yet Elsewhere
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{AuhFgQpPTJzUNempBYcZW5141K2.QX4QTN0wiM2gjNzEzW}`

```
hacker@paths~position-yet-elsewhere:~$ cd /challenge
hacker@paths~position-yet-elsewhere:/challenge$ ./run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:/challenge$ cd /
hacker@paths~position-yet-elsewhere:/$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{AuhFgQpPTJzUNempBYcZW5141K2.QX4QTN0wiM2gjNzEzW}
hacker@paths~position-yet-elsewhere:/$

```

The flag was revealed after changing `directories` once.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,

## References
I just used the problem statement as my reference
```
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now we can see what the ~ was in the prompt! It shows the current path that your shell is located at.

This challenge will requires us to execute the /challenge/run program from a specific path (which it will tell you). we'll need to cd to that directory before rerunning the challenge program.

```


# 6. Implicit relative paths, from /
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{UGKAkn08GILWqjvZZmKZum4vrlH.QX5QTN0wiM2gjNzEzW}`

```
hacker@paths~implicit-relative-paths-from-:/$ pwd
/
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{UGKAkn08GILWqjvZZmKZum4vrlH.QX5QTN0wiM2gjNzEzW}
hacker@paths~implicit-relative-paths-from-:/$


```

The flag was revealed after using the `relative part`.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,
I learnt how to use relative path and what is relative path
## References
I just used the problem statement as my reference
```
You'll need to run /challenge/run using a relative path while having a current working directory of /. For this level, I'll give you a hint. Your relative path starts with the letter c 😊
However, the current working directory does matter for relative paths.

A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to your current working directory (cwd).
Your cwd is the directory that your prompt is currently located at.
This means how you specify a particular file, depends on where the terminal prompt is located

```

# 7. Explicit relative paths, from /
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{kK4arUN2rEzp0eFL6HxaGfR-J4S.QXwUTN0wiM2gjNzEzW}`

```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kK4arUN2rEzp0eFL6HxaGfR-J4S.QXwUTN0wiM2gjNzEzW}
hacker@paths~explicit-relative-paths-from-:/$

```

The flag was revealed after using the `relative part`.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,
I learnt how to use relative path and what is relative path
## References
I just used the problem statement as my reference
```
You'll need to run /challenge/run using a relative path while having a current working directory of /. For this level, I'll give you a hint. Your relative path starts with the letter c 😊
However, the current working directory does matter for relative paths.

A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to your current working directory (cwd).
Your cwd is the directory that your prompt is currently located at.
This means how you specify a particular file, depends on where the terminal prompt is located
Of course, if your current working directory is /, the above relative paths are equivalent to the above absolute paths.

```

# 8. Implicit relative path 
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{wbbey_HTbdeCh7CAHif2BYV36Kn.QXxUTN0wiM2gjNzEzW}`

```
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wbbey_HTbdeCh7CAHif2BYV36Kn.QXxUTN0wiM2gjNzEzW}
hacker@paths~implicit-relative-path:/challenge$

```

The flag was revealed after using the `relative part`.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,
I learnt how to use relative path and what is relative path
## References
I just used the problem statement as my reference
```
This will not invoke /challenge/run. This is actually a safety measure: if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities! As a result, the above commands will yield the following error:
```
 
# 9. Home sweet home 
The challenge prompted me to change the directories and again to invoke after changing the directories. 

## My Solve
**Flag:** `pwn.college{gxVWWpnDCH3z0XXgMXIark9-aum.QXzMDO0wiM2gjNzEzW}`

```
hacker@paths~home-sweet-home:~$ /challenge/run
You must provide an argument to /challenge/run when you invoke it!
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{gxVWWpnDCH3z0XXgMXIark9-aum.QXzMDO0wiM2gjNzEzW}
hacker@paths~home-sweet-home:~$

```

The flag was revealed after using the `relative part`.

## What I learned
I learnt how to change the directories and
I learnt to execute program after changing the directories,
I learnt how to use relative path and what is relative path
I learnt how to do expansion of file
## References
I just used the problem statement as my reference
```
This will not invoke /challenge/run. This is actually a safety measure: if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities! As a result, the above commands will yield the following error:
In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:

Your argument must be an absolute path.
The path must be inside your home directory.
Before expansion, your argument must be three characters or less.
Again, you must specify your path as an argument to /challenge/run as so:
```
