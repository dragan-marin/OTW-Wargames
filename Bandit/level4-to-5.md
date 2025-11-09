# OverTheWire Bandit – Level 4 → 5

**Goal**: Find the only human-readable file among several in the `inhere` directory.

**Commands & Output**:
```bash
$ ls
inhere

$ cd inhere

$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09

$ file ./-file0*
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

$ cat ./-file07
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

Explanation:

There are 10 files named -file00 to -file09.
Names start with -, so use ./-file0* to avoid file interpreting them as options.
file command identifies file types.
Only -file07 is ASCII text → contains the password.
Key trick: Use file to find human-readable files.
