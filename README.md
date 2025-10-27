# OTW-BanditGame

Personal notes, hints, and scripts for the OverTheWire Bandit wargame.

## OverTheWire — Bandit Walkthrough (Personal Notes)

This repository contains my personal notes, hints, scripts, and learnings while solving the OverTheWire Bandit wargame. It may contain spoilers (including passwords). Use at your own discretion.

---

## Level 0 — Connect to the Server

Goal
- Connect to the Bandit server via SSH.

Key concepts
- To connect using `ssh` you need:
  - Server IP / hostname
  - Username
  - Password

SSH syntax
- Basic SSH syntax:
```bash
ssh username@host
```

Example (Bandit Level 0)
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
# Password for this initial connection: bandit0
```

Notes
- Once connected, the objective for Level 0 is to access the file that contains the password for the next level. Common commands to explore files are `ls`, `cat`, and `file`.
- This repository is for personal documentation and learning — expect spoilers (passwords, solutions) in the notes for each level.

Spoiler / Level 1 password (if you're looking for it)
```
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```


