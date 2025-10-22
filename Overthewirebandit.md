### Over The Wire Bandit Game

## First step
- Log into the server via: ssh bandit0@bandit.labs.overthewire.org -p 2220
- Password: bandit0
### Level 0 -> Level 1
- `cat "readme"`
- Password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
### Level 1 -> Level 2
- ssh bandit1@bandit.labs.overthewire.org -p 2220
- `cat ./-`
- Password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
### Level 2 -> Level 3
- ssh bandit2@bandit.labs.overthewire.org -p 2220
- `cat -- "--spaces in this filename--"`
- Password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
### Level 3 -> Level 4
- ssh bandit3@bandit.labs.overthewire.org -p 2220
- `cd inhere`
- `ls -a`
- `cat "...Hiding-From-You"`
- Password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
### Level 4 -> Level 5
- ssh bandit4@bandit.labs.overthewire.org -p 2220
- `file./*`
- `cat ./-file07`
- Password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
### Level 5 -> Level 6
- ssh bandit5@bandit.labs.overthewire.org -p 2220
- `find -readable -size 1033c ! -executable`
- `cat "./maybehere07/.file2"`
- Password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
### Level 6 -> Level 7
- ssh bandit6@bandit.labs.overthewire.org -p 2220
- `find / -user bandit7 -group bandit6 -size 33c 2>/dev/null`
- `cat "/var/lib/dpkg/info/bandit7.password"`
- Password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
### Level 7 -> Level 8
- ssh bandit7@bandit.labs.overthewire.org -p 2220
- `cat "data.txt" | grep millionth`
- Password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
### Level 8 -> Level 9
- ssh bandit8@bandit.labs.overthewire.org -p 2220
- `cat data.txt | sort | uniq -u`
- Password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
### Level 9 -> Level 10
- ssh bandit9@bandit.labs.overthewire.org -p 2220
- `cat "data.txt" | strings | grep =`
- Password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
### Level 10 -> Level 11
- ssh bandit10@bandit.labs.overthewire.org -p 2220
- `cat "data.txt" | base64 -d`
- dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
### Level 11 -> Level 12
- ssh bandit11@bandit.labs.overthewire.org -p 2220
- `cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'`
- Password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4



