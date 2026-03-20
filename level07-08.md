\# Bandit Level 7 → 8



\## Goal

The password is stored in data.txt next to the word "millionth".



\## Steps

ssh bandit7@bandit.labs.overthewire.org -p 2220

grep "millionth" data.txt



\## Password found

dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc



\## Notes

\- grep searches for a pattern inside a file

\- grep "word" file returns the line containing that word



