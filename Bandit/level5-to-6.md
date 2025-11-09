# Bandit Level 5 → 6

**Goal**: Find a file that is exactly 1033 bytes, not executable, and read it.

**Commands & Output**:
```bash
$ ls
inhere

$ cd inhere

$ find inhere -size 1033c ! -executable
inhere/maybehere07/.file2

$ cat inhere/maybehere07/.file2
HWasnPhctq9AVKe0dmK45nXy20CvUa6EG

Explanation:

ls shows the inhere directory.
cd inhere enters it.
find inhere -size 1033c ! -executable searches for a file that is exactly 1033 bytes and not executable.
Only one file matches: inhere/maybehere07/.file2.
cat reads it → password for bandit6.
