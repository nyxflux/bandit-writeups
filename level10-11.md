\# Bandit Level 10 → 11



\## Goal

The password is stored in data.txt encoded in base64.



\## Steps

ssh bandit10@bandit.labs.overthewire.org -p 2220

base64 -d data.txt



\## Password found

dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr



\## Notes

\- base64 -d : decodes a base64 encoded file

\- Base64 encodes binary data into readable ASCII characters

