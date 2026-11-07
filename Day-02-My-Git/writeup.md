# Day 02 – MY GIT

**Platform:** picoCTF 2026  
**Category:** General Skills  
**Difficulty:** Easy

### Challenge Description

"I have built my own Git server with my own rules!"

The challenge involved interacting with a custom Git server and following its instructions to submit a `flag.txt` file.

### What I did

1. Cloned the remote Git repository using SSH.
2. Inspected the repository and its commit history.
3. Configured the Git author name and email as instructed.
4. Created and staged `flag.txt`.
5. Committed the file.
6. Updated the remote URL after the challenge instance restarted.
7. Pushed the commit to the remote server and received the flag.

### Commands I learned

| Command | Purpose |
|---|---|
| `git clone` | Download a remote repository |
| `git log --oneline --all` | View commit history |
| `git config user.name` | Set commit author name |
| `git config user.email` | Set commit author email |
| `git add` | Stage changes |
| `git commit` | Save changes |
| `git remote -v` | View remote URLs |
| `git remote set-url` | Update remote URL |
| `git push` | Upload commits |

### Key Takeaway

Learned how Git repositories work, how commits store author information, and how to push changes to a remote Git server using SSH.
