\# Bandit 16 → 17



\## Goal

retrieve the credentials by submitting the password of the current level to a port on localhost in the range 31000–32000 using SSL/TLS — only one port returns credentials, the others echo back whatever is sent



\## Steps

ssh bandit16@bandit.labs.overthewire.org -p 2220



nmap -sV -p 31000-32000 localhost



openssl s\_client -connect localhost:31790

kSkvUpMQ71BYyCM4GBPvCvT1BfWRy0Dx



nano pvt16.key



chmod 600 pvt16.key



ssh -i pvt16.key bandit17@bandit.labs.overthewire.org -p 2220



\## Password found

EReVavePLFHtFlFsjn3hyzMlvSuSAcRD



\## Notes

\- nmap -sV = detects services running on each port (ssl and echo)

\- port 31790 = only SSL port that returns an RSA private key instead of echoing

\- the key is saved locally on your machine (not in /tmp on the server)

\- chmod 600 = required, SSH refuses keys with overly open permissions

\- ssh -i = specifies the private key + connects directly to the remote server

