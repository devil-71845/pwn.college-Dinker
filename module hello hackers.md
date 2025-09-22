# 1. Intro to Commands
The challenge prompted me to invoke my first command on the bash script, 
The command `whoami` was introduced.

## My Solve
**Flag:** `pwn.college{s1PKdUBiyYB4opuDso_8Gn2xkCW.QX3YjM1wiM2gjNzEzW}`

In the problem statement, it was provided that, using the 'hello' command if we are able to bring that hello output then we would be getting the flag
```
hacker@hello~intro-to-commands:~$ echo hello
hello
hacker@hello~intro-to-commands:~$ whoami
hacker
hacker@hello~intro-to-commands:~$ hello
Success! Here is your flag:
pwn.college{s1PKdUBiyYB4opuDso_8Gn2xkCW.QX3YjM1wiM2gjNzEzW}
hacker@hello~intro-to-commands:~$
```

## What I learned
I learnt to invoke my first command,
I learnt to invoke `whoami`,
The problem required me to run the command 'hello', which lead me to the flag.

## References
The problem statement was the reference used.
```
Here, the user executed the whoami command, which simply prints the username (hacker) to the terminal. When the command terminates, the shell once again displays the prompt, ready for the next command.here I used echo hello thinking I would be getting hello as output and i'll be getting flag but it was meant to be a wrong method.It was the only thing which I did is wrong.

In this level, invoke the hello command to get the flag! Keep in mind: commands in Linux are case sensitive: hello is different from HELLO.
```


# 2. Intro to Arguments
The challenge prompted me to use arguments with commands,
The command "echo" was introduced.

## My solve
**Flag:** `pwn.college{8msslstPYrln-pmWFoIK0Sk6891.QX4YjM1wiM2gjNzEzW}`

I was provided in the problem statement that using the `hackers` argument with the `hello` command would prompt the flag.

```
hacker@hello~intro-to-arguments:~$ echo hackers
hackers
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{8msslstPYrln-pmWFoIK0Sk6891.QX4YjM1wiM2gjNzEzW}
hacker@hello~intro-to-arguments:~$ pwn.college{8msslstPYrln-pmWFoIK0Sk6891.QX4YjM1wiM2gjNzEzW}
```

## What I learned
I learnt how to add arguments to commands,
I learnt how to use echo command, and the use of using the echo command,`
The problem required to me invoke the `hello` command with a specified argument to find the flag.

## References
The problem statement provided was used as the reference
```
Let's look at echo with multiple arguments:

hacker@dojo:~$ echo Hello Hackers!
Hello Hackers!
hacker@dojo:~$

In this case, the command was echo, and Hello and Hackers! were the two arguments to echo. Simple!

In this challenge, to get the flag, you must run the hello command (NOT the echo command) with a single argument of hackers. Try it now!
```


# 3. Command History
The challenge prompted me to check the command history. 

## My Solve
**Flag:** `pwn.college{ExYCvq5c36M-XkbR0uaiJYks7y2.0lNzEzNxwiM2gjNzEzW}`

```
hacker@hello~command-history:~$ the flag is pwn.college{ExYCvq5c36M-XkbR0uaiJYks7y2.0lNzEzNxwiM2gjNzEzW}
```

The flag was revealed after pressing `up arrow` key once.

## What I learned
I learned how to check the command history,
By pressing, the `up` and `down` keys, I can jump back and forward between the already used commands.

## References
I just used the problem statement as my reference
```
You're going to type a lot of commands, and typing everything from scratch can be annoying. Luckily, the shell saves the history of every command you execute.

You can scroll through those saved commands with the up/down arrow keys, and we'll practice that in this challenge. This challenge will inject the flag into your history. Bring up a terminal, hit the up arrow, and grab it! In other challenges, the history will contain the log of the commands you've run, so if you need to run a similar command again, you can use the arrow keys to scroll through and find it!
