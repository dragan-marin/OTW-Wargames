# Bandit Level 10 → 11

**Goal**: The password is stored in `data.txt` encoded in Base64. Decode it.

**Commands & Output**:
```bash
$ ls
data.txt

$ base64 data.txt
VkdobElIQmhjM04zYjNKa0lHbHpJR1IwVWpFM00yWmFTMkl3VWxKelJFWlRSM05uTWxKWGJuQk9W
bW96Y1ZKeUNnPT0K

$ base64 -d data.txt
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

Explanation:

data.txt contains Base64-encoded text.
base64 data.txt shows the encoded string (no decoding).
base64 -d data.txtdecodes it → reveals the password.
Password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
