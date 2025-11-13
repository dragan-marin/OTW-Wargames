# Bandit Level 11 → 12

**Goal**: The password in `data.txt` is rotated by 13 places (ROT13).

**Commands & Output**:
```bash
$ ls
data.txt

$ cat data.txt
Gur cnffjbeq vf 7k16JArUVv5LxVuJfsSVdbbtaHGlw9D4

Solution using CyberChef:

Pasted the string into CyberChef
Used ROT13 with "Rotate lower case chars" and "Rotate upper case chars"
Output: The password is 7x16WNeH1i5YkIhWsfFIqoognUTyj9Q4

Explanation:

The text is ROT13 encoded (each letter shifted by 13 positions).
Instead of using tr, I used CyberChef – a web tool for decoding.
Result: 7x16WNeH1i5YkIhWsfFIqoognUTyj9Q4
