# Initialise the database

$ msfdb init

# Base commands

- help
- search
- use
- set

# Lunch Metasploit

$ msfconsole

# The base command for searching

search

# Command to select a module as the active module

use

# View information about either a specific module or just the active one

info

# Communicat with a host

connect

# Command to change the value of a variable

set

# Command to change the value of a variable globally


setg

# View the value of a specific variable

get

# Change the value of a variable to null

unset

# Show variables and their values

show options

# Set console output to save to a file

spool

# Store the settings/active datastores from Metasploit to a settings file

save

# Module holds all of the exploit code

Exploit

# Module contains the various bits of shellcode to execute following exploitation

Payload

# Module is most commonly used in scanning and verification machines are exploitable

Auxiliary

# Module for looting and pivoting

Post

# Commonly utilized in payload obfuscation, module allows to modify the 'appearance' of exploit such that may avoid signature detection

Encoder

# Module is used with buffer overflow and ROP attacks

NOP

# Command to load different modules

load

# Feed results of nmap directly into database

db_nmap -sV -vv <ip>

# Show what information collected in the database

hosts

# Show services

services

# Command to Metasploit keep track of discovered vulnerabilities

vulns

# Check your IP

ip addr

# Run the exploit

run -j

# List all of sessions

sessions

# Interact with a target session

sessions -i SESSION_NUMBER

## The spool service is traditionally very stable and restarts pretty quickly in the case that we crash it
### The spool process will always match the architecture of your system
spoolsv.exe 

# Command to transfer into a process

migrate <PID>

# Command to find out more information regarding the current user running the process we are in

getuid

# Finding more information out about the system itself

sysinfo

#  Load mimikatz (The new version of mimikatz is referred to as 'kiwi' in metasploit)

load kiwi

# Privileges of our current user

getprivs

# Transfer files to victims computer

upload

# Run a Metasploit module

run <module name>

# Command to show the networking information and interfaces on the victims machine

ipconfig

# Combination to background

ctrl + z
