# Step 1

Username: garry
Password: letmein

# Flag 1

ls
cat flag1.txt

Username: bob
Password: linuxrules

# Flag 2

su -l bob
cat flag2.txt

# Flag 3

ls -la
cat .bash_history

# Flag 4

crontab -l

# Flag 5

find / -name "flag5*" 2>/dev/null
cat /lib/terminfo/E/flag5.txt

# Flag 6

find / -name "flag6*" 2>/dev/null
grep "c9" /home/flag6.txt 

# Flag 7

ps -ef

# Flag 8

tar -xzf flag8.tar.gz
cat flag8.txt

# Flag 9

cat /etc/hosts

# Flag 10

cat /etc/passwd

# Flag 11

cat .bashrc

# Flag 12

cat /etc/update-motd.d/00-header

# Flag 13

cd flag13
diff *

# Flag 14

cat /var/log/flagtourteen.txt 

# Flag 15

cat /etc/lsb-release

# Flag 16

cd /media/f/l/a/g/1/6/is
ls

# Flag 17

Username: alice
Password: TryHackMe123

su -l alice
cat flag17

# Flag 18

cat .flag18

# Flag 19

cat -n flag19
head -n 2345 flag19
 sed -n 2345p flag19

# Flag 20

cat flag20

ends on "=" means it's base64

base64 -d flag20

# Flag 21

find / -name "flag21.php" 2>/dev/null
vim /home/bob/flag21.php 

# Flag 22

convert hex to ascii

xxd -r -p flag22

# Flag 23

reverse a string

rev flag23

# Flag 24

strings /home/garry/flag24

# Flag 26

find / -xdev -type f -print0 2>/dev/null | xargs -0 grep -E '^[a-z0-9]{32}$' 2>/dev/null

# Flag 27

find / -name "flag27*" 2>/dev/null


List the allowed (and forbidden) commands for the invoking user
sudo -l

sudo cat /home/flag27

# Flag 28

uname -r

# Flag 29

cat /home/garry/flag29 | tr -d ' '

# Flag 30

curl localhost

# Flag 31

mysql -u root -p

SHOW DATABASES;

# Flag 32

USE <database_name>
SHOW tables;
DESCRIBE flags
SELECT flag from flags;

# Flag 33
open a new termnal window on your machine
scp alice@10.10.60.185:/home/alice/flag32.mp3 ./Desktop

# Flag 34

env

# Flag 35

cat /etc/group

# Flag 36

find / -name "flag36" 2>/dev/null
cat /etc/flag36