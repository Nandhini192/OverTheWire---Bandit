# OverTheWire---Bandit# 

LEVEL 0:

Goal: Login to the Bandit server using SSH.

Command used:
ssh bandit0@bandit.labs.overthewire.org -p 2220
Password:bandit0

Result:Successfully logged in to bandit level 0.

ls
cat readme
Result:Password for the next level obtained from the readmefile.
exit


LEVEL 1

Goal: Find the password stored in a file.

Commands used:
ssh bandit1@bandit.labs.overthewire.org -p 2220
Password:use the password found in level 0.

Result:Successfully logged in to bandit level 1.

ls
cat ./-
Result:shows the password for next level
exit
