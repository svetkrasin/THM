# Clear the screen

ctrl + l

# Connet to another machine 

$ ssh <username>@<ip>

# Check name of the machine

$ hostname


# Change the user on the machine

$ su <username>

# Redirect output to file '>'

$ echo hello > file

//it will ovveride all data stored before

# Append output to a file

$ echo hello >> file

# Execute commands in queue '&&' (behaves as logical and)

$ ls && echo hello

# Run a command on background '&'

$ sleep 42 &

# Set an enviroment variable

$ export <varname>=<value>

# Use output of a command as input '|'

$ ls | grep <filename>

# Execute commands in order ';'

$ dsdfdsfsd; ls

# Set the diffent permissions for a file

$ chmod <permissons> <file>

| Digit |                     Meaning                     |
| ----- | ----------------------------------------------- |
|   1   | That file can be executed                       |
|   2   | That file can be written to                     |
|   3   | That file can be executed and written to        |
|   4   | That file can be read                           |
|   5   | That file can be read and executed              |
|   6   | That file can be written to and read            |
|   7   | That file can be read, written to, and executed |

<permissons>=UserGroupEveryone

# Change the user and group for any file

$ chown <user><:group> <filename>

# Move files

$ mv <file> <destination>

# Copy files

$ cp <file> <destination>

# Create hard and symbolic links

$ ln <source> <destination>

# Find files

$ find <variables>

# Find data inside of data

$ grep <string> <file1> <file2>...

$ grep <regular expression> <file>

# Run a command as another user

$ sudo -u <username> <command>

# Add user

$ adduser <username>

# Add group

$ addgroup <groupname>

# Add user to a group

$ usermod -a -G  <groups seperated by commas> <user>

# View basic information about a user

id <username>

# Work in nano

^<key> = ctrl + <key>

# See all the users on a system

/etc/passwd - Stores user information

# All the passwords of these users

/etc/shadow

# Sudo permissions of every user on the system

/etc/sudoers

# All software installed

/usr

# System critical files

/bin

/sbin

# The Linux miscellaneous directory

/var -A myriad of processes store data in there

# All the binaries you're able to run

$PATH

# A list of user created precesses

$ ps

to view list of all system precesses

$ ps -ef

# Stop precesses

$ kill <PID>

# Open file explorer in place 

$ nautilus

# Check runing services

systemctl -t service --all

# Check status of a service

systemctl status <service_name1> <service_name2>

# Restart service

systemctl restart <service_name1> <service_name2>

# Stop service

systemctl stop <service_name> <service_name2>

# Disable a service

systemctl disable <service_name1> <service_name2>
