# OverTheWire Bandit – Level 3 → 4

**Goal**: Find the password hidden in a file with a strange name inside the `inhere` directory.

**Commands & Output**:
```bash
$ ls -a
. .. .bash_logout .bashrc inhere .profile

$ cd inhere/

$ ls -a
. .. ...Hiding-From-You

$ cat ...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

Explanation:

ls -a shows all files, including hidden ones (starting with .).
inhere is a directory → cd inhere to enter.
Inside, ls -a reveals a file named ...Hiding-From-You.
cat ...Hiding-From-You displays the password for bandit4.
Key trick: Hidden files and directories are revealed with ls -a.
                                        
