# 1. Learning From Documentation.
The challenge prompted me to invoke /challenge/challenge with --giveflag argument on the bash script, 

## My Solve
**Flag:** `pwn.college{ki7bq5IR1zBAapwp4RDUbvQbEVQ.QX0ITO0wiM2gjNzEzW}`

In the problem statement, The correct usage of programs depends, in a large part, on the proper specification of arguments to them. Recall the -a of ls -a in the hidden files challenge of the Basic Commands module: that -a was an argument that told ls to list out hidden files as well as non-hidden files. Because we wanted to list out hidden files, invoking ls with the -a argument was the correct way to use it in our scenario.
```
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{ki7bq5IR1zBAapwp4RDUbvQbEVQ.QX0ITO0wiM2gjNzEzW}
hacker@man~learning-from-documentation:~$


```

## What I learned
I learnt to invoke argument with /challenge/challenge command,
I learnt to invoke `/challenge/challenge --giveflag`,
The problem required me to run the command '/challenge/challenge with argument --giveflag', which displayed me the flag.

## References
The problem statement was the reference used.
```
The program for this challenge is /challenge/challenge, and you'll need to invoke it properly in order for it to give you the flag. Let's pretend that this is its documentation...

```

# 2. Learning Complex Usage.
The challenge prompted me to invoke /challenge/challenge with --printfile argument on the bash script, to print the flag file.

## My Solve
**Flag:** `pwn.college{kUeEX-krAeFrNF0o-DxxIRfMnLR.QX1ITO0wiM2gjNzEzW}`


Welcome to the documentation for /challenge/challenge! This program allows you to print arbitrary files to the terminal, when given the --printfile argument. The argument to the --printfile argument is the path of the flag to read. For example, /challenge/challenge --printfile /challenge/DESCRIPTION.md will print out the description of the level!.

```
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{kUeEX-krAeFrNF0o-DxxIRfMnLR.QX1ITO0wiM2gjNzEzW}
hacker@man~learning-complex-usage:~$

```

## What I learned
I learnt to invoke argument with /challenge/challenge command,
I learnt to invoke `/challenge/challenge --printfile`,
The problem required me to run the command '/challenge/challenge with argument --printfile', which displayed me the flag.

## References
The problem statement was the reference used.
```
The program for this challenge is /challenge/challenge, and you'll need to invoke it properly in order for it to give you the flag...

```


# 3. Reading Manuals.
The challenge prompted me to invoke man command on the bash script, to print the manual for particular command.

## My Solve
**Flag:** `pwn.college{UxO9H2FKyZii1UPKrB_ihD-vvW4.QX0EDO0wiM2gjNzEzW}`


This level introduces the man command. man is short for manual, and will display (if available) the manual of the command you pass as an argument!.

```
hacker@man~reading-manuals:~$ man challenge // manual will be opened from which we will select the argument to display the file.
hacker@man~reading-manuals:~$ /challenge/challenge --xyiiri 921
Correct usage! Your flag: pwn.college{UxO9H2FKyZii1UPKrB_ihD-vvW4.QX0EDO0wiM2gjNzEzW}
hacker@man~reading-manuals:~$

```

## What I learned
I learnt to invoke argument with man command,
I learnt to invoke `man`,
The problem required me to run the command 'man with /challenge/challenge', which displayed me the flag.

## References
The problem statement was the reference used.
```
Manpages are stored in a centralized database. If you're curious, this database lives in the /usr/share/man directory, but you never need to interact with it directly: you just query it using the man command. The arguments to the man command aren't file paths, but just the names of the entries themselves (e.g., you run man yes to look up the yes manpage, rather than man /usr/bin/yes, which would be the actual path to the yes program but would result in man displaying garbage).
```

# 4. Searching Manuals.
The challenge prompted me to invoke me to scroll up/down with PgUp/PgDn keys and search the manual with / and search for a option which will give a flag by reading the challenge man page.
## My Solve
**Flag:** `pwn.college{csyddWCRSPvj6TMAHaG9KGRpwy9.QX1EDO0wiM2gjNzEzW}`


You can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, you can hit n to go to the next result and N to go to the previous result. Instead of /, you can use ? to search backwards!.

```
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --lqsoojh
Initializing...
Correct usage! Your flag: pwn.college{csyddWCRSPvj6TMAHaG9KGRpwy9.QX1EDO0wiM2gjNzEzW}
hacker@man~searching-manuals:~$


```

## What I learned
I learnt to invoke man command,
I learnt to invoke `man`,
The problem required me to run the command 'man with /challenge/challenge' with suitable true argument, which displayed me the flag.

## References
The problem statement was the reference used.
```
Manpages are stored in a centralized database. If you're curious, this database lives in the /usr/share/man directory, but you never need to interact with it directly: you just query it using the man command. The arguments to the man command aren't file paths, but just the names of the entries themselves (e.g., you run man yes to look up the yes manpage, rather than man /usr/bin/yes, which would be the actual path to the yes program but would result in man displaying garbage).

```

# 5. Searching For Manuals.
The challenge prompted me to invoke me to man command to man itself to view the manual and use the according argument of man [man -k] alongwith /challenge/challenge in order to get flag

## My Solve
**Flag:** `pwn.college{gyfjH1TBhtVVoeiVLHukV4IOVqO.QX2EDO0wiM2gjNzEzW}`


This level is tricky: it hides the manpage for the challenge by randomizing its name. Luckily, all of the manpages are gathered in a searchable database, so you'll be able to search the man page database to find the hidden challenge man page! To figure out how to search for the right manpage, read the man page manpage by doing: man man!.

```
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
gyfjhtoeiu (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man gyfjhtoeiu
hacker@man~searching-for-manuals:~$ /challenge/challenge --gyfjht 142
Correct usage! Your flag: pwn.college{gyfjH1TBhtVVoeiVLHukV4IOVqO.QX2EDO0wiM2gjNzEzW}
hacker@man~searching-for-manuals:~$

```

## What I learned
I learnt to invoke man  command to view manual of man command,
I learnt to invoke `man`,
The problem required me to run the command 'man with man' with suitable true argument, which displayed me the flag after running with /challenge/challenge.

## References
The problem statement was the reference used.
```
HINT 1: man man teaches you advanced usage of the man command itself, and you must use this knowledge to figure out how to search for the hidden manpage that will tell you how to use /challenge/challenge

HINT 2: though the manpage is randomly named, you still actually use /challenge/challenge to get the flag!

```

# 6. Helpful programs.
The challenge prompted me to invoke me to --help argument with any program (challenge)


## My Solve
**Flag:** `pwn.college{gyXWaM9sCEhFAXrVDQ5Fr4T7pUY.QX3IDO0wiM2gjNzEzW}`


Some programs don't have a man page, but might tell you how to run them if invoked with a special argument. Usually, this argument is --help, but it can often be -h or, in rare cases, -?, help, or other esoteric values like /? (though that latter is more frequently encountered on Windows).

In this level, you will practice reading a program's documentation with --help. Try it out!

```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 954
hacker@man~helpful-programs:~$ /challenge/challenge -g 954
Correct usage! Your flag: pwn.college{gyXWaM9sCEhFAXrVDQ5Fr4T7pUY.QX3IDO0wiM2gjNzEzW}
hacker@man~helpful-programs:~$

```

## What I learned
I learnt to invoke  --help  kind of special arguments along with programs.
I learnt to invoke `--help`,
The problem required me to run the argument `--help`` and other arguments along with /challenge/challenge.

## References
The problem statement was the reference used.
```
Some programs don't have a man page, but might tell you how to run them if invoked with a special argument. Usually, this argument is --help, but it can often be -h or, in rare cases, -?, help, or other esoteric values like /? (though that latter is more frequently encountered on Windows).

In this level, you will practice reading a program's documentation with --help. Try it out!
```

# 7. Help for Builtins  
The challenge prompted me to use the `help` command to find the documentation for builtins, through that finding the flag.  
  
## My Solve  
**Flag:** `pwn.college{U3aWvsTWcYjXSOVGYYvUvxPLMTd.QX0ETO0wiM2gjNzEzW}`  
  
I used `help` to find the usage of `challenge` command which was a builtin for this challenge. Using that I found the correct argument and value to put with that argument.  
```  
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "U3aWvsTW".
hacker@man~help-for-builtins:~$ challenge --secret U3aWvsTW
Correct! Here is your flag!
pwn.college{U3aWvsTWcYjXSOVGYYvUvxPLMTd.QX0ETO0wiM2gjNzEzW}

hacker@man~help-for-builtins:~$

```  
  
## What I Learned  
I learnt what are builtins. Builtins are commands which are built in to the shell and are handled internally by the shell.   
The usage of `help` with builtins.  
  
## References  
The problem statement provided was used as the reference.  
```  
Some good information! In this challenge, we'll practice using help to look up help for builtins. This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it!  
```
