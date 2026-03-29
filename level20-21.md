\# Bandit 20 → 21



\## Goal

use the setuid binary suconnect — it connects to a port on localhost, reads a password, and if it matches bandit20's password, it sends back the password for bandit21



\## Steps

ssh bandit20@bandit.labs.overthewire.org -p 2220



***Terminal 1:***



nc -l -p 3333

0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO



***Terminal 2:***



./suconnect 3333



\## Password found

EeoULMCra2q0dSkYj561DX7s1CpBuOBt



\## Notes

\- nc -l -p 3333 = opens a listener on port 3333 (waits for a connection)

\- suconnect = setuid binary that connects to the port, reads the password, and verifies it

\- if the password is correct → suconnect returns the password of bandit21 in terminal 1

\- if the password is incorrect → suconnect closes the connection without returning anything

\- 2 terminals are needed

