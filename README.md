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

*(No further output shown in the transcript for this exact command — the user subsequently tried the correct username form.)*

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




