# OverTheWire Bandit – Level 2 → 3

**Goal**: Read a file with spaces and leading dashes in the name.

**Commands & Output**:
```bash
$ ls -la
-rw-r----- 1 bandit3 bandit2 33 Oct 14 09:26 --spaces in this filename--

$ cat ./--spaces\ in\ this\ filename--
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

Explanation:
File name starts with --, which cat interprets as an option. Use ./-- to force it to treat the rest as a filename. Escape spaces with \ or use quotes.
