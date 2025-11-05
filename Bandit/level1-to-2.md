# OverTheWire Bandit – Level 1 → 2

**Goal**: Read a file named `-` (dash), which is interpreted as stdin by `cat`.

**Commands & Output**:
```bash
$ ls
-

$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx

Explanation:
The file is named -, so cat - would read from stdin (keyboard). Using ./- treats it as a regular file path and displays the password for bandit2.
