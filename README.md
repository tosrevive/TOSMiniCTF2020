# TOS Mini Capture the Flag (CTF) 2020

This is a mini capture the flag event for TempleOS.  In this repostitory there is a RedSea ISO file ```TOSMiniCTF.ISO.C``` with 5 benign TempleOS binaries 1.BIN.Z thru 5.BIN.Z.  Each is an ahead of time compiled short simple program less than 400 bytes, which asks the user for a password and reports if the password is correct.  The first one is intended to be easy, the rest may require some more work.  There is only one correct answer for each and the password for each is composed of less than 20 printable ASCII characters.  This CTF is geared toward people who know assembly / debugging / reverse engineering assembly code.

# Getting started

- 1) Transfer ```TOSMiniCTF.ISO.C``` to you TempleOS machine or VM
- 2) Mount it  ```MountFile("D:/path/to/TOSMiniCTF.ISO.C");```
- 3) Change to the mounted drive ```Cd("M:/")``` (assuming this is the first file you mounted)
- 4) Load and crack the password for each of them.  Ex:```Load("1");```, ```Load("2");```, etc

# Getting credit for the answer

When you have an answer create an issue with a SHA256 sum of the correct password to prove to the world you were the first person to crack it.

Example: 

If the password is T3mple05Rock5! the SHA256 sum could be calculated on Linux with:

```echo -n "T3mple05Rock5!" | sha256sum```

Be sure not to include newlines in your hash (that's what the -n is for).



