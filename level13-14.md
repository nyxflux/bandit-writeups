\# Bandit Level 13 → 14



\## Goal

Log into bandit14 using a private SSH key instead of a password.



\## Steps

ssh bandit13@bandit.labs.overthewire.org -p 2220



scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .

chmod 400 sshkey.private

ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220



cat /etc/bandit\_pass/bandit14



\## Password found

MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS



\## Notes

\- scp copies a file from a remote server to your local machine

\- -i specifies the SSH key to use instead of a password

\- chmod 400 makes the key readable only by you

\- The key was an RSA private key stored in bandit13's home directory

