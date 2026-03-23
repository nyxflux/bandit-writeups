\# Bandit 15 → 16



\## Goal

retrieve by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption



\## Steps

ssh bandit15@bandit.labs.overthewire.org -p 2220



openssl s\_client -connect localhost:30001

8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo



\## Password found

kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx



\## Notes

\-openssl s\_client = encrypted connection (SSL/TLS)

\-(-connect) = choose the target (IP and port)

