\# Bandit 17 → 18



\## Goal



compare two files to find the only line modified between the two in order to get the password



\## Steps

ssh bandit17@bandit.labs.overthewire.org -p 2220



ls



grep -vxFf passwords.old passwords.new



\## Password found

x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO



\## Notes

\- grep -vxFf = find only what is different between two files

