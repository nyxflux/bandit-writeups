\# Bandit Level 12 → 13



\## Goal

The password is stored in data.txt as a hexdump 

of a file compressed multiple times.



\## Steps



\### Setup

ssh bandit12@bandit.labs.overthewire.org -p 2220

cd /tmp

mkdir newprinpfiles

cd newprinpfiles

cp /home/bandit12/data.txt .



\### Convert hexdump to binary

xxd -r data.txt > data.bin



\### Decompress chain

mv data.bin data.gz

gunzip data.gz          # → gzip



mv data data.bz2

bzip2 -d data.bz2       # → bzip2



mv data data.gz

gunzip data.gz          # → gzip



tar -xf data            # → tar → data5.bin

tar -xf data5.bin       # → tar → data6.bin



mv data6.bin data6.bz2

bzip2 -d data6.bz2      # → bzip2



tar -xf data6           # → tar → data8.bin



mv data8.bin data8.gz

gunzip data8.gz         # → gzip → data8



cat data8               # → password



\## Password found

FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn



\## Notes

\- Use `file` after each step to identify compression type

\- Rename file with correct extension before decompressing

\- xxd -r converts hexdump back to binary



