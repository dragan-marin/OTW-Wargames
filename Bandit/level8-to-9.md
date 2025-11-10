# Bandit Level 8 → 9

**Goal**: Find the password — the only line that appears exactly once in `data.txt`.

**Commands & Output**:
```bash
$ sort data.txt | uniq -u
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

Explanation:

data.txt has many repeated lines.
sort data.txt sorts all lines.
uniq -u shows only lines that appear exactly once.
Only one line matches → that's the password for bandit9.


