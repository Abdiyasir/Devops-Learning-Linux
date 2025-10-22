# Devops-Learning-Linux
This repository covers the useful common commands in linux and the different topics I have covered.
## Common Commands
### Navigation & Directory Management
| Command    | Description                                |
| ---------- | ------------------------------------------ |
| `pwd`      | Show current working directory             |
| `ls`       | List directory contents                    |
| `ls -l`    | List with file details (permissions, size) |
| `ls -a`    | Show hidden files                          |
| `cd <dir>` | Change directory                           |
| `cd ..`    | Go up one level                            |
| `cd ~`     | Change to home directory                       |
### File & Directory Management
| Command                   | Description                     |
| ------------------------- | ------------------------------- |
| `mkdir <name>`            | Create a directory              |
| `mkdir -p path/to/newdir` | Create nested directories       |
| `rmdir <dir>`             | Remove an empty directory       |
| `rm <file>`               | Remove a file                   |
| `rm -r <dir>`             | Remove a directory and contents |
| `cp <source> <destination>`         | Copy a file                     |
| `cp -r <source> <destination>`      | Copy a directory                |
| `mv <source> <destination>`         | Move or rename files/folders    |
| `touch <file>`            | Create an empty file            |
### Viewing Files
| Command            | Description            |
| ------------------ | ---------------------- |
| `cat <file>`       | Display file contents  |
| `head -n 5 <file>` | Show first 5 lines     |
| `tail -f <file>`   | Follow a log file live |
### Search
| Command                             | Description               |
| ----------------------------------- | ------------------------- |
| `grep "text" file`                  | Search inside a file      |
| `find . -name "file.txt"`           | Search for a file by name starting (.) and looks in all subdirectories also.|
| `find /path -type d -name "folder"` | Search for a directory named folder inside /path and all the subdirectories |
### Redirection and Text Processing Commands
| Command | Description                |  
| ------- | -------------------------- | 
| `>`     | Replaces the content of the file |                                
| `>>`    | Adds content to the end of the file      |                               
| `sort`  | Sort lines                 |                                
| `uniq`  | Removes consecutive duplicate lines from a file |                                
| `wc -l` | Count lines                |                               
### Permissions
| Command              | Description              |
| -------------------- | ------------------------ |
| `chmod 755 file`     | Change file permissions - Owner can read, write and execute - Group & Others can read and execute |
| `chmod +x script.sh` | Make a script executable |
| `chown user file`    | Changes ownership of a file so that 'user' becomes the new owner |

