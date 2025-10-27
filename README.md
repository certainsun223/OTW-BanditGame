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

* convert this README to a single-file (e.g. `Bandit-Level-0-to-1-README.md`) and provide it as a downloadable file, or
* produce similar READMEs for subsequent Bandit levels using transcripts you provide.
