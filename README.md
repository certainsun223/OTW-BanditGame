# OTW-BanditGame — Complete Walkthrough

Personal notes, hints, and exact commands used while solving OverTheWire — **Bandit**. **Contains spoilers / passwords** 

---

## Quick legend

* `ssh -p 2220 banditN@bandit.labs.overthewire.org` → connect as `banditN`
* Commands are listed in order; final output in each section is the password for the next level.

---

## Level 0 ➜ 1

```bash
ssh -p 2220 bandit0@bandit.labs.overthewire.org
ls
cat readme
exit
```

**Password:** `ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If`

---

## Level 1 ➜ 2

```bash
ssh -p 2220 bandit1@bandit.labs.overthewire.org
ls
cat ./-
```

**Password:** `263JGJPfgU6LtdEvgfWU1XP5yac29mFx`

---

## Level 2 ➜ 3

```bash
ssh -p 2220 bandit2@bandit.labs.overthewire.org
ls
cat -- "--spaces in this filename--"
```

**Password:** `MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx`

---

## Level 3 ➜ 4

```bash
ssh -p 2220 bandit3@bandit.labs.overthewire.org
ls
cd inhere
find
cat ./...Hiding-From-You
```

**Password:** `2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ`

---

## Level 4 ➜ 5

```bash
ssh -p 2220 bandit4@bandit.labs.overthewire.org
cd inhere
ls -l
file ./*
cat ./-file07
```

**Password:** `4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw`

---

## Level 5 ➜ 6

```bash
ssh -p 2220 bandit5@bandit.labs.overthewire.org
cd inhere
find -size 1033c -readable ! -executable
cat ./maybehere07/.file2
```

**Password:** `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

---

## Level 6 ➜ 7

```bash
ssh -p 2220 bandit6@bandit.labs.overthewire.org
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

**Password:** `morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`

---

## Level 7 ➜ 8

```bash
ssh -p 2220 bandit7@bandit.labs.overthewire.org
ls
grep millionth data.txt
```

**Password:** `dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc`

---

## Level 8 ➜ 9

```bash
ssh -p 2220 bandit8@bandit.labs.overthewire.org
ls
sort data.txt | uniq -u
```

**Password:** `4CKMh1JI91bUIZZPXDqGanal4xvAg0JM`

Alternative:

```bash
strings data.txt | grep ==
```

**Password (alt):** `FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey`

---

## Level 10 ➜ 11

```bash
ssh -p 2220 bandit10@bandit.labs.overthewire.org
ls
base64 -d data.txt
```

**Password:** `dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr`

---

## Level 11 ➜ 12

```bash
ssh -p 2220 bandit11@bandit.labs.overthewire.org
ls
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

**Password:** `7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4`

---

## Level 12 ➜ 13

**Goal:** `data.txt` is a hexdump of a repeatedly compressed file. Work in `/tmp`.

```bash
ssh -p 2220 bandit12@bandit.labs.overthewire.org
mkdir -p /tmp/bandit12_work
cd /tmp/bandit12_work
xxd -r /home/bandit12/data.txt > data.bin
file data.bin
# Repeatedly unpack with correct suffix:
mv data.bin data.bin.gz && gunzip data.bin.gz
mv data.bin data.bin.bz2 && bunzip2 data.bin.bz2
mv data.bin data.bin.tar && tar -xf data.bin.tar
# repeat until ASCII
cat data8.bin  # or final ASCII file
```

**Password:** `FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn`

---

## Level 13 ➜ 14

**Goal:** use private SSH key for `bandit14`.

```bash
ssh -p 2220 bandit13@bandit.labs.overthewire.org
chmod 600 sshkey.private
ssh -i sshkey.private -p 2220 bandit14@localhost
cat /etc/bandit_pass/bandit14
```

**Password:** `MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS`

---

## Level 14 ➜ 15

**Goal:** submit current password to localhost:30000 via netcat.

```bash
ssh -p 2220 bandit14@bandit.labs.overthewire.org
echo "MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS" | nc localhost 30000
```

**Password:** `8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo`

