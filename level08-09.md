\# Bandit Level 8 → 9



\## Goal

The password is the only line that appears once in data.txt.



\## Steps

ssh bandit8@bandit.labs.overthewire.org -p 2220

sort data.txt | uniq -u



\## Password found

4CKMh1JI91bUIZZPXDqGanal4xvAg0JM



\## Notes

\- sort : sorts lines alphabetically (required before uniq)

\- uniq -u : only prints lines that appear exactly once

\- | (pipe) : sends output of one command into another



