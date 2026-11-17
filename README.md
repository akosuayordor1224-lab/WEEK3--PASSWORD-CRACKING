# Week 3 - Password Cracking

**Name:** Diana Yordor
Date:17 November 2026  

## What I Did
I had 2 locked PDFs. I found the password for both. I opened them. I got the flag.

Flag = "Congratulations! You have captured your flag."

---

## PM2 -Easy Way

**PDF:** My Locked PDF1 for NW Tools
**Password:** `1qaz2wsx`

**Steps:**
1. Uploaded PDF to Hash Calculator
2. Got the hash - it starts with `$pdf$`
3. Pasted hash into Password Cracker
4. Cracker gave me the password: `1qaz2wsx`
5. Opened PDF with that password - It worked!

---

## PM1 - Johnny Way

**PDF:** My Locked PDF1
**Password:** `password1`

**Steps:**
1. Downloaded John and Johnny
2. Told Johnny where John is: `run/john.exe`
3. Saved hash as `hash1.txt` in PowerShell
4. Opened `hash1.txt` in Johnny
5. Clicked Start new attack
6. Johnny gave me the password: `password1`
7. Opened PDF with that password - It worked!

---

## Problems I Had
- Johnny could not find John at first. I fixed it in Settings.
- Word made my hash file messy. PowerShell with ASCII made it clean.
- I have 4 PDFs. I learned to check the exact name.

## What I Learned
- A PDF has a hash. A hash hides the password.
- You can crack a hash to find the password.
- You can crack online (PM2) or on your laptop with Johnny (PM1).

**Flags: 2/2 - PM1 + PM2 DONE**
