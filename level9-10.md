\# Bandit Level 9 → 10



\## Goal

The password is stored in data.txt among human-readable strings, preceded by several = characters.



\## Steps

ssh bandit9@bandit.labs.overthewire.org -p 2220

strings data.txt | grep '='



\## Password found

FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey



\## Notes

\- strings : extracts human-readable text from a binary file

\- grep '=' : filters lines containing the = character



