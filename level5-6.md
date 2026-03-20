\# Bandit Level 5 → 6



\## Goal

The password is stored in a file somewhere under inhere, human-readable, 1033 bytes, not executable.



\## Steps

ssh bandit5@bandit.labs.overthewire.org -p 2220

cat ./maybehere07/.file2



\## Password found

HWasnPhtq9AVKe0dmk45nxy20cvUa6EG



\## Notes

\- find -size 1033c can locate files by exact size

\- -readable and ! -executable are useful find filters

