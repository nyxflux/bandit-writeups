\# Bandit Level 11 → 12



\## Goal

The password is stored in data.txt where all letters have been rotated by 13 positions (ROT13).



\## Steps

ssh bandit11@bandit.labs.overthewire.org -p 2220

cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'



\## Password found

7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4



\## Notes

\- tr : translates/replaces characters

\- ROT13 shifts each letter by 13 positions in the alphabet

\- Applying ROT13 twice gives back the original text





