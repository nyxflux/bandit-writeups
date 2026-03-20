\# Bandit Level 1 → 2



\## Goal

The password is stored in a file called - located in the home directory.



\## Steps

ssh bandit1@bandit.labs.overthewire.org -p 2220

cat ./-



\## Password found

263JGJPfgU6LtdEvgfWU1XP5yac29mFx



\## Notes

\- ./ prefix is needed to read a file named - (otherwise the shell interprets it as stdin)

