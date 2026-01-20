# Cybersecurity-Internship-Task4 

# Password Security & Cracking Analysis

## Environment
- OS: Ubuntu or Kali linux
- Tools: John the Ripper, Hashcat
- Wordlist: rockyou.txt

## Hash Generation
$ echo -n "password" | md5sum

### John the Ripper

$ john --wordlist=rockyou.txt hash.txt
$ john --show hash.txt

### Hashcat

$ hashcat -m 0 -a 0 hash.txt rockyou.txt
$ hashcat --show -m 0 hash.txt

(screenshots are attached for hashing and cracking the hashed weak passwords(text))
### Attacks

- Dictionary Attack
- Brute Force Attack

## Result

- Weak MD5 hashes cracked successfully
- Demonstrates importance of strong passwords and MFA
