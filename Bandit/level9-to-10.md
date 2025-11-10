# Bandit Level 9 → 10

**Goal**: Find the password preceded by several `=` characters in a binary file.

**Commands & Output**:
```bash
$ ls
data.txt

$ strings data.txt | grep "="
FB`=
c\5D=
========== the
?/=l
=Uc1
=vG*2P
========== password
k=ezG
E========== is
=%r_
.?=Dm
O&A=n
5========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
=*^Y
=L3jT
q<=,
'QHE=
+=NBf

Explanation:

data.txt is a binary file → use strings to extract readable text.
The password is preceded by several = characters.
grep "=" shows all lines with =.
We look for the line with the longest sequence of = and readable text after it.
The line 5========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey contains the password:
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
