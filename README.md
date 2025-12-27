# OverTheWire---Bandit# 

LEVEL 0:

Goal: Login to the Bandit server using SSH.

Commands:

ssh bandit0@bandit.labs.overthewire.org -p 2220                                                                                  
Password:bandit0

Result:Successfully logged in to bandit level 0.






LEVEL 0 - LEVEL 1

Goal: Find the password stored in a file.

Commands:

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

Commands:

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

Commands:

ssh bandit2@bandit.labs.overthewire.org -p 2220

Enter the password obtained from Level 1.

ls
(--spaces in this filename)

cat ./--spaces\ in\ this\ filename--

The output is the password for Bandit Level 3

exit

Result:Successfully obtained the password for Level 3.






Level 3 - Level 4

Goal: The password for the next level is stored in a hidden file in the inhere directory.

Commands:

ssh bandit3@bandit.labs.overthewire.org -p 2220

Enter the password obtained from Level 2.

cd inhere means move into the folder named inhere so you can access the files inside it.

cd inhere

ls -a(. .. ...Hiding-From-You)

cat ...Hiding-From-You

The output is the password for Bandit Level 4

exit

The output is the password for Bandit Level 4






Level 4 -Level 5

Goal:The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

Commands:

ssh bandit4@bandit.labs.overthewire.org -p 2220

Enter the password obtained from the Level 3

Type ls to see inhere

Type cd inhere

Type ls

many files like:

-file00  -file01  -file02  ...

Type file ./*

output like:

./-file00: data
./-file01: data
./-file07: ASCII text

ASCII text is human-readable file

Type cat ./-file07

The output is the password for Bandit Level 5.

exit.

Result:Successfully obtained the password for Level 5.






Level 5 - Level 6

Goal:The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

Commands:

ssh bandit5@bandit.labs.overthewire.org -p 2220

Enter the password obtained from the Level 4

Type ls to see inhere

Type cd inhere

Type find . -type f -size 1033c ! -executable

output be like ./maybehere07/.file2

Type cat ./maybehere07/.file2

The output is the password for Bandit Level 6.

exit.

Result:Successfully obtained the password for Level 6.























