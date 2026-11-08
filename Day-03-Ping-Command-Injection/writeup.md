# Day 03 – Ping Command Injection

**Platform:** CyLab Security Academy  
**Category:** General Skills  
**Difficulty:** Easy

### Challenge Description

"Can you make the server reveal its secrets? It seems to be able to ping Google DNS, but what happens if you get a little creative with your input?"

### Investigation

The challenge provided a terminal connection to a remote server using Netcat. The server requested an IP address and claimed that it only allowed `8.8.8.8`.

I first entered the permitted IP address to understand the normal behaviour of the application.

I then experimented with additional input to investigate how the server handled user input.

### Commands Used

| Command | Purpose |
|---|---|
| `nc` | Connect to the remote challenge server |
| `whoami` | Identify the user executing commands |
| `ls` | List files and directories |
| `cat` | Display file contents |
| `;` | Separate commands in a shell |

### What I Discovered

1. The server successfully executed the ping command.
2. Using a semicolon, I was able to execute an additional command.
3. `whoami` revealed that commands were running as `ctf-player`.
4. `ls` revealed two files: `flag.txt` and `script.sh`.
5. I used `cat flag.txt` to display the challenge flag.

### Key Learning

This challenge introduced me to **OS Command Injection**, a vulnerability that occurs when an application handles user input unsafely while constructing system commands.

I learned how shell command separators work, how to inspect a remote environment and how to investigate a potential vulnerability rather than relying on the application's input restrictions.

### Skills Practised

- Linux command-line fundamentals
- Netcat
- Shell command execution
- OS Command Injection
- Basic remote environment enumeration

