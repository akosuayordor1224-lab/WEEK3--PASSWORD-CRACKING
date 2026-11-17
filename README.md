# Week 3 — Password Cracking Lab Report

**Author:** YORDOR DIANA MARY
**Date:** November 2026  
**Status:** ✅ Completed

## What This Lab Is About

I was given locked PDFs. I could not open them because I did not know the password.

My job was to:
1. Find the hidden code of the PDF — this is called a **hash**
2. Crack the hash to find the **password**
3. Open the PDF with the password and get the **flag**

Flag message:
> Congratulations! You have captured your flag.

## What I Used

- **Johnny** — a simple tool with buttons for cracking passwords
- **John the Ripper** — the engine that does the cracking
- **Networkwalks Hash Calculator** — to get the hash from the PDF
- **Networkwalks Password Cracker** — to crack the hash online
- **PowerShell** — to save the hash as a clean file

## My Results

| Lab | What I Cracked | Password I Found |
|---|---|---|
| **PM2** | My Locked PDF1 (NW Tools) | `1qaz2wsx` |
| **PM1** | My Locked PDF1 | `password1` |

Both PDFs opened. Both flags captured.

---

## PM2 — The Easy Way (Online)

1. I uploaded the PDF to Hash Calculator. It gave me the hash.
2. I copied the hash.
3. I pasted the hash into Password Cracker and clicked Crack.
4. It gave me the password: `1qaz2wsx`
5. I opened the PDF with that password. It worked.


![PM2 Result]

---

## PM1 — The Johnny Way (On My Laptop)

1. I downloaded John and Johnny from Openwall and installed them.
2. In Johnny, I went to Settings and pointed it to `john.exe`. Johnny found John.
3. I saved my hash as `hash1.txt` using PowerShell, so the file was clean.
4. I opened `hash1.txt` in Johnny and clicked Start new attack.
5. Johnny found the password: `password1`
6. I opened the PDF with that password. It worked.


---

## Problems I Had

**1. Johnny could not find John.**
→ I fixed it by setting the path to `john.exe` in Johnny Settings.

**2. Johnny showed strange symbols.**
→ Word made the file messy. I saved it again in PowerShell as ASCII, and it worked.

**3. I had 4 PDFs with similar names.**
→ I learned to check the exact file name before I open it.

---

## What I Learned

- A locked PDF has a hash. The hash hides the password.
- You can crack a hash online (PM2) or on your own laptop (PM1).
- A clean file is important. If the file is messy, Johnny cannot read it.
- To prove a password is correct, you must open the PDF with it.

## Conclusion

Both labs are done. I found both passwords and captured both flags.

**✅ Week 3 Complete**
