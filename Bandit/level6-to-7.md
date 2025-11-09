# Bandit Level 6 → 7

**Goal**: Find a file anywhere on the system owned by `bandit7`, group `bandit6`, exactly 33 bytes, and read it.

**Commands & Output**:
```bash
$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password

$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

Explanation:

find / searches the entire filesystem.
-user bandit7 -group bandit6 → file must belong to user bandit7 and group bandit6.
-size 33c → exactly 33 bytes.
2>/dev/nullhides all "Permission denied" errors so we only see the real result.
Only one file matches → contains the password for bandit7.
