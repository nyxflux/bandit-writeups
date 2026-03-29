\# Bandit 19 → 20



\## Goal

use the setuid binary present in the home directory to read the password of the next level



\## Steps

ssh bandit19@bandit.labs.overthewire.org -p 2220



ls -la



./bandit20-do cat /etc/bandit\_pass/bandit20



\## Password found

0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO



\## Notes

\- setuid = special permission that executes the binary with the rights of its owner (bandit20)

\- the s in -rwsr-x--- indicates that the setuid bit is activated

\- bandit20-do = any order placed runs as bandit20

\- cat /etc/bandit\_pass/bandit20 = readable only by bandit20

