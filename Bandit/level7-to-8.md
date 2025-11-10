# Bandit Level 7 → 8

**Goal**: Find the line containing "millionth" in `data.txt`.

**Commands & Output**:
```bash
$ cat | grep "millionth" data.txt
millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

Explanation:

cat | grep reads input and filters for "millionth".
Only one line matches → password is dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc.
Alternative (cleaner): grep "millionth" data.txt does the same without cat.
