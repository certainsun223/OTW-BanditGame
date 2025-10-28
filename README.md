# OTW-BanditGame

Personal notes, hints, and scripts for the OverTheWire Bandit wargame.

## OverTheWire — Bandit Walkthrough (Personal Notes)

This repository contains my personal notes, hints, scripts, and learnings while solving the OverTheWire Bandit wargame. It may contain spoilers (including passwords). Use at your own discretion.

---
# OverTheWire Bandit — Level 0 → Level 1

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 0 → level 1**.



---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Attempt to connect (no username specified):

```bash
ssh bandit.labs.overwire.org -p 2220
```



2. Connect with the `bandit0` username (correct form):

```bash
ssh -p 2220 bandit0@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* SSH prompts for password.
* On successful login the server displays the OverTheWire/Bandit welcome ASCII art and help text (omitted here for brevity in the README). Example header shown during login:

```
                        _                     _ _ _   
                       | |__   __ _ _ __   __| (_) |_
                       | '_ \ / _` | '_ \ / _` | | __|
                       | |_) | (_| | | | | (_| | | |_
                       |_.__/ \__,_|_| |_|\__,_|_|\__|

                     This is an OverTheWire game server.
           More information on http://www.overthewire.org/wargames
```

3. List files in the home directory:

```bash
ls
```

**Output:**

```
readme
```


4. Display the contents of the `readme` file with `cat`:

```bash
cat readme
```

**Output (the file contents):**

```
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walkthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```

7. Exit the SSH session:

```bash
exit
```

**Output:**

```
logout
Connection to bandit.labs.overthewire.org closed.
```

---

## Password obtained for Level 0 → Level 1

**Password:** `ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If`

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit0@bandit.labs.overthewire.org` → `ls` →  `cat readme` → `exit`.
* The password for the next level is shown in the `readme` file and captured above.




---







# OverTheWire Bandit — Level 1 → Level 2

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 1 → level 2**.

> Note: this file reproduces the session transcript you provided and formats it into a clear, step-by-step README. Do not share the password publicly (OverTheWire asks players not to post spoilers).

---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Connect with the `bandit1` username:

```bash
ssh -p 2220 bandit1@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* SSH prompts for the password and on success shows the OverTheWire/Bandit welcome banner.

2. List files in the home directory:

```bash
ls
```

**Output:**

```
-
```


3. Display the contents of the file named `-` in the current directory using `cat` with a path that avoids treating `-` as an option:

```bash
cat ./-
```

**Output (the file contents, which is the password):**

```
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```


---

## Password obtained for Level 1 → Level 2

**Password:** `263JGJPfgU6LtdEvgfWU1XP5yac29mFx`

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit1@bandit.labs.overthewire.org` → `ls` → `cat ./-`.
* The password for the next level is the contents of the file named `-`, displayed with `cat ./-` and captured above.








# OverTheWire Bandit — Level 2 → Level 3

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 2 → level 3**.

> Note: this file reproduces the session transcript you provided and formats it into a clear, step-by-step README. Do not share the password publicly (OverTheWire asks players not to post spoilers).

---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Connect with the `bandit2` username:

```bash
ssh -p 2220 bandit2@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* First password attempt failed with "Permission denied, please try again." Then a second password was entered and login succeeded, showing the Bandit welcome banner.

2. List files in the home directory:

```bash
ls
```

**Output:**

```
--spaces in this filename--
```

3. Display the contents of the file whose name contains spaces. Because the filename contains spaces, use quoting (and `--` to stop option parsing) when passing it to `cat`:

```bash
cat -- "--spaces in this filename--"
```

**Output (the file contents, which is the password):**

```
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```

4. (Optional) Exit the SSH session:

```bash
exit
```

**Output:**

```
logout
Connection to bandit.labs.overthewire.org closed.
```

---

## Password obtained for Level 2 → Level 3

**Password:** `MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx`

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit2@bandit.labs.overthewire.org` → `ls` → `cat -- "--spaces in this filename--"` → `exit`.
* The password for the next level is the contents of the file named `--spaces in this filename--`, displayed with `cat` and captured above.

---





# OverTheWire Bandit — Level 3 → Level 4

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 3 → level 4**.

> Note: this file reproduces the session transcript you provided and formats it into a clear, step-by-step README. Do not share the password publicly (OverTheWire asks players not to post spoilers) unless you're using it privately for the game.

---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Connect with the `bandit3` username:

```bash
ssh -p 2220 bandit3@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* SSH prompts for the password and on success shows the OverTheWire/Bandit welcome banner.

2. List files in the home directory:

```bash
ls
```

**Output:**

```
inhere
```


3. Change into the relative directory `./inhere`:

```bash
cd ./inhere
```

**Output / prompt:**

```
bandit3@bandit:~/inhere$
```


4. Run `find` to search the directory (no args):

```bash
find
```

**Output:**

```
.
./...Hiding-From-You
```

5. Display the hidden file named `...Hiding-From-You` using `cat`:

```bash
cat ./...Hiding-From-You
```

**Output (the file contents, which is the password):**

```
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```

6. (Optional) Exit the SSH session:

```bash
exit
```

**Output:**

```
logout
Connection to bandit.labs.overthewire.org closed.
```

---

## Password obtained for Level 3 → Level 4

**Password:** `2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ`

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit3@bandit.labs.overthewire.org` → `ls` → `cd ./inhere` → `find` → `cat ./...Hiding-From-You` → `exit`.
* The password for the next level is the contents of the hidden file `...Hiding-From-You` found by `find` and displayed with `cat`.

---





# OverTheWire Bandit — Level 4 → Level 5

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 4 → level 5**.

> Note: this file reproduces the session transcript you provided and formats it into a clear, step-by-step README. Do not share the password publicly (OverTheWire asks players not to post spoilers) unless you're using it privately for the game.

---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Connect with the `bandit4` username:

```bash
ssh -p 2220 bandit4@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* SSH prompts for the password and on success shows the OverTheWire/Bandit welcome banner.

2. List files in the home directory:

```bash
ls
```

**Output:**

```
inhere
```

3. Change into the `inhere` directory and list files:

```bash
cd ./inhere
ls
```

**Output:**

```
-file00  -file02  -file04  -file06  -file08
-file01  -file03  -file05  -file07  -file09
```

4. Use `find` to list files (shows same names):

```bash
find
```

**Output:**

```
.
./-file02
./-file04
./-file08
./-file00
./-file07
./-file06
./-file01
./-file03
./-file05
./-file09
```

5. Use `ls -l` to inspect file sizes and permissions:

```bash
ls -l
```

**Output (truncated):**

```
total 40
-rw-r----- 1 bandit5 bandit4 33 Oct 14 09:26 -file00
-rw-r----- 1 bandit5 bandit4 33 Oct 14 09:26 -file01
...
-rw-r----- 1 bandit5 bandit4 33 Oct 14 09:26 -file07
...
```

6. Use `du` to check disk usage:

```bash
du
```

**Output:**

```
44	.
```

7. Use `file` to determine file types:

```bash
file ./*
```

**Output:**

```
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
```

8. Display the contents of the readable text file `-file07` (note the leading dash — use `./-file07` to avoid option parsing):

```bash
cat ./-file07
```

**Output (the file contents, which is the password):**

```
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```

9. (Optional) Exit the SSH session:

```bash
exit
```

**Output:**

```
logout
Connection to bandit.labs.overthewire.org closed.
```

---

## Password obtained for Level 4 → Level 5

**Password:** `4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw`

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit4@bandit.labs.overthewire.org` → `ls` → `cd ./inhere` → `ls`/`find`/`ls -l` → `file ./*` → `cat ./-file07` → `exit`.
* The password for the next level is the contents of `-file07`, displayed with `cat` and captured above.

---




# OverTheWire Bandit — Level 5 → Level 6

This README documents the exact commands used (in order), their outputs, and the password obtained for **Bandit level 5 → level 6**.  (Only the useful commands are included.)

---

## Prerequisites

* SSH client (OpenSSH)
* Network access to `bandit.labs.overthewire.org` on port `2220`

---

## Commands, outputs, and password

1. Connect to the level:

```bash
ssh -p 2220 bandit5@bandit.labs.overthewire.org
```

*(SSH password prompt and successful login banner are shown in the session; omitted here for brevity.)*

2. List and enter the `inhere` directory:

```bash
ls
cd ./inhere
ls
```

**Output (directory listing):**

```
maybehere00  maybehere04  maybehere08  maybehere12  maybehere16
maybehere01  maybehere05  maybehere09  maybehere13  maybehere17
maybehere02  maybehere06  maybehere10  maybehere14  maybehere18
maybehere03  maybehere07  maybehere11  maybehere15  maybehere19
```

3. Use `find` to inspect contents recursively (optional verbose listing):

```bash
find ./*
```

**Output:** (truncated — shows all `maybehereXX` directories and their files)

```
./maybehere00
./maybehere00/.file1
... (many entries)
./maybehere19/-file3
```

4. Detailed listing to check permissions and sizes:

```bash
ls -l
```

**Output:** (shows directories owned by `root:bandit5` — truncated)

```
total 80
drwxr-x--- 2 root bandit5 4096 Oct 14 09:26 maybehere00
...
drwxr-x--- 2 root bandit5 4096 Oct 14 09:26 maybehere19
```

5. Find the readable non-executable file of size 1033 bytes and show it. The `find` command used was:

```bash
find -size 1033c -readable ! -executable
```

**Output:**

```
./maybehere07/.file2
```

6. Display the password (contents of the found file):

```bash
cat ./maybehere07/.file2
```

**Output (the password for the next level):**

```
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```

7. (Optional) exit the SSH session:

```bash
exit
```

---

## Password obtained for Level 5 → Level 6

**Password:** `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

---





# Bandit Level 6 → 7

**SSH into Bandit6:**

```bash
ssh -p 2220 bandit6@bandit.labs.overthewire.org
```

**List files (default is empty):**

```bash
ls
ls -l
ls -la
```

**Goal:** Find the file owned by `bandit7`, group `bandit6`, size 33 bytes (password for next level).

**Correct `find` command:**

```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
```

**Output (found file):**

```
/var/lib/dpkg/info/bandit7.password
```

**View the password for next level:**

```bash
cat /var/lib/dpkg/info/bandit7.password
```

**Password (Bandit7):**

```
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```





# OverTheWire Bandit — Level 7 → Level 8

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 7 → level 8**.

> Note: this file reproduces the session transcript you provided and formats it into a clear, step-by-step README. Do not share the password publicly (OverTheWire asks players not to post spoilers).

---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Connect with the `bandit7` username:

```bash
ssh -p 2220 bandit7@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* SSH prompts for the password and on success shows the OverTheWire/Bandit welcome banner.

2. List files in the home directory:

```bash
ls
```

**Output:**

```
data.txt
```

3. Attempt to `cd` into the file (demonstrated mistakes in the transcript):

```bash
cd data.txt
cd ./data.txt
```

**Output:**

```
-bash: cd: data.txt: Not a directory
```

4. Inspect the file and its ownership/size:

```bash
ls -l
head -n 10 data.txt
```

**Output (truncated):**

```
total 4088
-rw-r----- 1 bandit8 bandit7 4184396 Oct 14 09:26 data.txt

# head -n 10 data.txt
Krishnamurti	qw8nXVhFD5bTB8g5qt8MQqgmvwKjGe3B
twice	ShdFKBKXyAD4vabgf4gRFGsSSTfd8JAQ
sprucest	d64AVQB1lcJvA3dMlluHBPaKjlRRMOeL
crosses	zlRV9E0QNc3CBQlzE8GLh3Kax2JIo901
apprehending	Rh0DHqfvw8Ze1v82wyf4j0K6czbLlcNX
clutters	hAUm5ZUYJXxhIk1Uu8OinBU75HMk6SPH
prisoners	8FNhExxaVru0aA1eCXrAMbyOyrIo0F5M
Renee	VYfLkTfaEgJA7oVfmTr3spGORUCSoook
tweak	cGziWWRhIALtBq6vHS2B8Fw1qlob8byT
Lin	njF0006Ac01XsliZRdBHE1lQpyQxMYuW
```

5. Find the line containing the word `millionth` using `grep` and display it:

```bash
grep millionth data.txt
```

**Output:**

```
millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit7@bandit.labs.overthewire.org` → `ls` → `ls -l`/`head -n 10 data.txt` → `grep millionth data.txt`.
* The password for the next level is the second column on the `millionth` line in `data.txt` and is captured above.


















# OverTheWire Bandit — Level 8 → Level 9

This README documents the exact commands used (in order), their outputs, and the password obtained at the end of the level for **Bandit level 8 → level 9**.

> Note: this file reproduces the session transcript you provided and formats it into a clear, step-by-step README. Do not share the password publicly (OverTheWire asks players not to post spoilers).

---

## Prerequisites

* SSH client installed (OpenSSH).
* Network access to `bandit.labs.overthewire.org` on port `2220`.

---

## Session steps (commands, order, and outputs)

1. Connect with the `bandit8` username:

```bash
ssh -p 2220 bandit8@bandit.labs.overthewire.org
```

**Output / interaction** (condensed):

* SSH prompts for the password and on success shows the OverTheWire/Bandit welcome banner.

2. List files in the home directory:

```bash
ls
```

**Output:**

```
data.txt
```

3. Use the `sort` and `uniq` command to find the unique line in the file:

```bash
sort data.txt | uniq -u
```

**Output:**

```
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

---

## Minimal summary

* Commands used in order: `ssh -p 2220 bandit8@bandit.labs.overthewire.org` → `ls` → `sort data.txt | uniq -u`.
* The password for the next level is the unique string returned by the final command.
