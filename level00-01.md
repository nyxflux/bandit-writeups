\# Bandit Level 0/1 



\## Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.



\## Steps

ssh bandit0@bandit.labs.overthewire.org -p 2220

ls 

cat readme



\## Passwords found

ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If



\## Notes 

ls = lists the files in the folder

cat = displays the contents of the file

Always use ls first to help you find your way

