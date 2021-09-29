# Invironment Variables

| Name | Default Value |
| %CD% | Current directory |
| %DATE% | Current date |
| %OS | Windows |
| %ProgramFiles% | C:\Program Files |
| %ProgramFiles)x86% | C:\Program Files (x86) |
| %TIME% | Current time |
| %USERPROFILE% | C:\Users{username} |
| %SYSTEMDRIVE% | C:\ |
| %SYSTEMROOT% | C:\Windows |

# CMD Commands

| Name | Action | Linux Counterpart |
| cd or chdir | Change directory | cd |
| dir | List contents of directory | ls |
| md or mkdir | Create directory | mkdir |
| copy | Copy file | cp |
| move | Move files | mv |
| del or erase | Delete files and directories | rm |
| rd or rmdir | Remove a directory if empty | rmdir |
| find | Search a file for specified string | grep |
| exit | Close CMD | exit |
| type | Show contents of specified file | cat |

# PowerShell Commands

| cmdlet | Function | Equivalent Command |
| Set-Location | Changes to specified directory | cd |
| Get-ChildItem | Returns current directory contents | ls, dir |
| New-Item | Makes new file or directory | mkdir, touch |
| Remove-Item| Deletes file or directory | rm, rmdir |
| Get-Location | Retrieves path to current directory | pwd |
| Get-Content | Returns file content | cat, type |
| Copy-Item | Copies a file from on locatin to another | cp |
| Move-Item | Moves item from one location to another | mv |
| Write-Output | Prints output | echo |
| Get-Alias | Shows aliases from the current session | alias |
| Get-Help | Retrieves information about command | man |
| Get-Process | Retrieves precesses running on mahine | ps |
| Stop-Process | Stops specific process | kill |
| Get-Service | Retrieves list of services | service --status-all |

# wmic precess

## list values from os wmic alias

wmic os get \value

## All user info, SID (Security Identifier), important directories, and files

wmic useraccount get name, sid, description

## The number of times all users have logged on, and last logon

wmic netlogin get caption, numberoflogons, lastlogon

## Windows update information

wmic qfe get caption, description, installedon, hotfixid

# Enumerate users

net user

# UserName password status

net user UserName

# Groups on the machine

net localgroup

# The current password policy

net accounts

# Create a regular user

net user UserName UserPassword \add

# Change password of an existin user

net user UserName *

# Add UserName to a group

net localgroup GroupName UserName \add

# List groups of a user

net user UserName

# Set password policies

gpedit

# DNS hosts file

C:\Windows\System32\drivers\etc\Hosts
