# OverTheWire---Bandit# 

LEVEL 0:

Goal: Login to the Bandit server using SSH.

Solution:

ssh bandit0@bandit.labs.overthewire.org -p 2220                                                                                  
Password:bandit0

Result:Successfully logged in to bandit level 0.



LEVEL 0 - LEVEL 1

Goal: Find the password stored in a file.

Solution:

ssh bandit1@bandit.labs.overthewire.org -p 2220

Password:bandit0

ls
(readme)

cat readme

The output is the password for Bandit Level 1

exit

Result:Successfully obtained the password for Level 1.



LEVEL 1 - LEVEL 2

Goal: The password for the next level is stored in a file called - located in the home directory.

Solution:

ssh bandit1@bandit.labs.overthewire.org -p 2220

Enter the Password obtained from the level 0

ls
( - )

cat ./-

The output is the password for Bandit Level 2

exit

Result:Successfully obtained the password for Level 2.




LEVEL 2 - LEVEL 3

Goal: The password for the next level is stored in a file called --spaces in this filename-- located in the home directory

Solution:

ssh bandit2@bandit.labs.overthewire.org -p 2220

Enter the password obtained from Level 1.

ls
(--spaces in this filename)

cat ./--spaces\ in\ this\ filename--

The output is the password for Bandit Level 3

exit

Result:Successfully obtained the password for Level 3.



