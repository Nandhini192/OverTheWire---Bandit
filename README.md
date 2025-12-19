# OverTheWire---Bandit# 

LEVEL 0:

Goal: Login to the Bandit server using SSH.

Command used:
ssh bandit0@bandit.labs.overthewire.org -p 2220
Password:bandit0

Result:Successfully logged in to bandit level 0.


LEVEL 0 - LEVEL 1

Goal: Find the password stored in a file.

Commands used:
ssh bandit1@bandit.labs.overthewire.org -p 2220
Password:bandit0

ls
cat readme
The output is the password for Bandit Level 1
exit

Result:Successfully obtained the password for Level 1.


LEVEL 1 - LEVEL 2

Goal: The password for the next level is stored in a file called - located in the home directory.

ssh bandit1@bandit.labs.overthewire.org -p 2220
Enter the Password obtained from the level 0

ls
cat ./-
The output is the password for Bandit Level 2
exit

Result:Successfully obtained the password for Level 2.

