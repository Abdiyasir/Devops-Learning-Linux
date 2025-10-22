# Introduction to Linux

Linux is an open-source operating system created by Linus Torvalds.
It is widely recognized for:
- 🛡️ Security – stable and less prone to viruses
- ⚙️ Flexibility – runs on almost any hardware or system
- 🌍 Community support – continuously improved by developers worldwide

### What is the Terminal?
- The Terminal is a command-line interface (CLI) that lets you interact with the operating system by typing commands, it's where you can navigate and automate tasks.

### Anatomy of a Linux Command
Commands generally follow this structure:
- `command [options] [arguments]`
- `ls -a Desktop`

### Introduction to the Shell
The shell acts as a bridge between you and the operating system, interpreting what you type and translating into system actions.
### Type of Shells
| Shell | Full Name                  | Key Features                                   |
| ----- | -------------------------- | ---------------------------------------------- |
| Bash  | Bourne Again Shell         | Default on most systems                        |
| Zsh   | Z Shell                    | Customizable, autocompletion, spell correction |
| Fish  | Friendly Interactive Shell | Syntax highlighting, suggestions               |
| Ksh   | Korn Shell                 | Enterprise compatibility                       |
| Sh    | Bourne Shell               | Simpler, classic shell                         |

### Superuser Access with sudo
- sudo stands for superuser do — it runs commands with administrative privileges.
- Example
- `sudo apt install <package>` | Install a new package
- `sudo !!` | Run the previous command again, but with sudo

### Managing Users
- Users can be created, switched, granted access & have access removed on linux.
- `sudo adduser newuser`
- `sudo passwd newuser`
- `su - newuser`
- `sudo usermod -aG sudo newuser`
- `sudo deluser newuser sudo`

### Managing Groups
- Groups can be created, have users added, users deleted & the group deleted
- `sudo groupadd devops`
- `sudo usermod -aG devops newuser`
- `sudo gpasswd -d newuser devops`
- `sudo groupdel devops`

### File Permissions
- Each file has three permission sets: user (owner), group, and others.
- Example:
- `-rwxr-xr--`
- r = read
- w = write
- x = execute
- '-' = no permissions
- File permission commands:
- `chmod u+x script.sh` | add execute for the user
- `chmod g+r file.txt` | add read for the group
- `chmod o-w file.txt` | remove write for others
- `chmod a+x run.sh` | make executable for all
- `chmod ug=rw,o=r file.txt` | specific permissions for the file — User & Group: read & write, Others: read only.
- `chmod ug=rw,o=r file.txt` | specific permissions for the file — User & Group: read & write, Others: read only.


### Numeric Mode for Permissions
| Number | Meaning              | Permissions |
| ------ | -------------------- | ----------- |
| 7      | Read, write, execute | rwx         |
| 6      | Read, write          | rw-         |
| 5      | Read, execute        | r-x         |
| 4      | Read                 | r--         |
| 0      | None                 | ---         |

### Changing Ownership
- Each file has an owner and a group.
- `sudo chown newuser file.txt` | Changes ownership of file.txt so that newuser becomes its owner.
- `sudo chgrp newgroup file.txt` | changes group ownership of file.txt so that the group admin becomes the new group associated with it
- `sudo chown newuser:newgroup file.txt` | Changes both the owner and the group of file.txt in one step.
- `sudo chown -R newuser:newgroup directory/` | recursively changes ownership of a directory and everything inside it — including all subdirectories and files. Owner becomes newuser & group becomes newgroup

### Standard Streams
Linux commands use three data streams:

- Standard Input (stdin) → What you type into a command.
- Standard Output (stdout) → The normal results a command prints.
- Redirect to a file with > (overwrite) or >> (append).
- Standard Error (stderr) → Where error messages go.
- Redirect to a file with 2> (overwrite) or 2>> (append).
- To redirect both output and errors, use &> or &>>.
- Send output to /dev/null to discard it.

### Environment Variable
- Environment variables define your shell environment and behavior.
- $PATH – directories searched for executables
- $HOME – user home directory
- $USER – username
- $SHELL – current shell
Temporary Variable Example:
- `sudo chown -R newuser:newgroup directory/` | creates an environment variable called MY_VAR with the value "hello".
- By default, variables you create (like MY_VAR) only last for the current terminal session.
To make them permanent, you add them to your shell config file — for example, .zshrc if you use Zsh.
- `export MY_VAR="hello" && source ~/.zshrc` | By default, variables you create (like MY_VAR) only last for the current terminal session. To make them permanent, you add them to your shell config file — for example, .zshrc.



