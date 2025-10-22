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




