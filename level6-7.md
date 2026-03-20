\# Bandit Level 6 → 7



\## Goal

The password is stored somewhere on the server, owned by user bandit7, group bandit6, 33 bytes.



\## Steps

ssh bandit6@bandit.labs.overthewire.org -p 2220

cat /var/lib/dpkg/info/bandit7.password



\## Password found

morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj



\## Notes

\- find / -user bandit7 -group bandit6 -size 33c searches the whole server

\- 2>/dev/null hides permission denied errors

