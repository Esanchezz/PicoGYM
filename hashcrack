# PicoCTF Gym: Hashcrack

## Objectives
- Figure out the flag for the lab
- Help understand the way the lab was created

## Findings
### Description of Lab
"A company stored a secret message on a server which got breached due to the admin using weakly hashed passwords. Can you gain access to the secret stored within the server?"<br>
When connecting to the lab, it deliberately gives the user the hash and to input the solved hash as the "password".<br>

### Solving the lab
I immediately opened up a web hash cracker.<br>
The website I used was "crackstation.net" and it had a very straight forward GUI.<br>
Website automatically solves each hash inputted as it supports LM, NTLM, md2, md4, md5, md5(md5_hex), md5-half, sha1, sha224, sha256, sha384, sha512, ripeMD160, whirlpool, MySQL 4.1+ (sha1(sha1_bin)), QubesV3.1BackupDefaults hashes, making it easier for users.<br>
The first hash ("482c811da5d5b4bc6d497ffa98491e38") was identified as a MD5 hash with the password being:"password123", which later led to the lab giving the user another hash.<br>
Inputting the next hash ("b7a875fc1ea228b9061041b7cec4bd3c52ab3ce3") was identified as a SHA-1 hash with the password being:"letmein", which later led to the lab giving the last hash.<br>
Inputting the last hash ("916e8c4f79b25028c9e467f1eb8eee6d6bbdff965f9928310ad30a8d88697745") was identified as a SHA-256 hash with the password being:"qwerty098", with the flag being given picoCTF{UseStr0nG_h@shEs_&PaSswDs!_36a1cf73}.<br>

### Things we can learn from this lab
What we can learn from this lab are a few things. <br>
There are different types of hash crackers available, a commonly used one is Hashcat with more scalable and specific controls for more use cases. I simply just used the one that was easiest and quick to understand this lab.<br>
We also learned some hashes that cyber security professionals should be able to recognize when seeing them. These hash functions are MD5, SHA-1, and SHA-256<br>
MD5 creates a 128-bit hash value with it's main use in cryptography. It is now no longer recommended as over the course of it's use, there were vulnerabilities found. It is, however, still used for database partitiioning and computing checksums to validate file transfers.<br>
SHA-1 stands for Secure Hash Algorithm, which is the first version of SHA. It generates 160-bit hash(20 bytes). It was also found to have vulnerabilities and is no longer considered to be less resistant to attack than MD5.<br>
SHA-256 outputs a 256-bit hash and it is currently the recommended algorithm for most applications due to it's strong resistance to attacks and it's widespread use in industry standards.<br>
Another thing to note is that the Website Crackstation has it's word list available which is 15 Gb. When using a hash cracker, usually the there isnt a preset wordlist, therefore you would need a wordlist for the application to solve the hashes.<br>

## Final Thoughts
I thought this lab was a very simple and fun lab to understand how hash crackers and hashes work.<br> It also brings to awareness how easy some passwords could be solved when using a complex wordlist.
