\# Bandit 17 → 18



\## Goal



compare two files to find the only line modified between the two in order to get the password



\## Steps

ssh bandit17@bandit.labs.overthewire.org -p 2220



ls 



grep -vxFf passwords.new  passwords.old



\## Password found

pGozC8kOHLkBMOaL0ICPvLV1IjQ5F1VA



\## Notes

\- grep -vxFf = find only what is different between two files

