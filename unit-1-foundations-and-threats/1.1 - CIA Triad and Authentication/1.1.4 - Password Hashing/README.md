# 1.1.4 - Password Hashing

## Lesson Objective(s):
- Recognize authentication vocabulary terms.
- Understand methods of secure password storage.
- Define hashing as a method of one-way conversion.

## Guiding Question(s):
- How are passwords stored on a system and what is password hashing?
Passwords aren’t stored as they are; the system turns them into a long, jumbled code using hashing. When you log in, your password is hashed again and matched with the stored code to see if it’s correct, keeping it safe from hackers.

### Lecture Notes
> From the course notes reviewed in class, take note on the material from this lesson as it relates to the Lesson Objectives and Guiding Question(s):
Windows machine- SAM registry hive holds all account details like usernames and passwords.

Passwords should never be stored in plain text.

MD5, SHA256 and SHA512 are commonly used hashing algorithms.

Linux: store usernames, passwords and some settings 

etc/shadow- hidden file used to store usernames, passwords and some settings remember only root usershave access.

The actual hashing algorithms are much more complex and do more than just performing arithmetic operations on relatively small numbers.

SALT- method of protecting against Rainbow Table Attacks.

Pass the hash attack- this attack does not try to crack the password instead attacker gets to the SAM hive or etc to dump the hashes from storage system.

Using special software, the attacker logs in the username and password hash instead of the text password.

### Application / Personal Research / Summary
> In your own words, write a summary of this lesson and connect it to yourself and the real-world. If needbe, do a rapid research on the topic to help with you summary
   
      Based on what I learned about this lesson was about hashing and how hackers try to guess your password by hashing. Also it is basically In this lesson, I learned about passwords, password hashing, and how systems keep data safe. Passwords aren’t stored as they are  instead, they are turned into scrambled codes using hashing so that even if someone steals the data which are the hackers , they cannot see the real password. This lesson is really important for me because I use passwords for my email, social media, and school accounts every day. In the real world, password hashing helps protect people from hackers, keeps personal information safe, and makes the internet a more secure place for everyone. In addition I wanna add that learning how to keep password safe is really important in real life so when it comes to virtual world like connecting with our phones and technologies we are safe and secured all the time.
...

### Vocabulary
> Include the vocabulary word(s) from this lesson with a defintion

Single Sign On- one authentication gives access to many servers or resources 

Passphrases- a string of words provides more protection than a strong password but users are resistant to typing and it is not mobile device friendly.

Hashing- a special mathemathical function that performs one-way conversion. Also it is intended as one way conversion. Once the algorithm is processed, the hashed password is stored by the system.

Hash collision- when two or more source data convert to the same hash value

Birthday Attack- in a group of 22 people the chance that two people share a birthday is greater than 50%.

Rainbow Tables- definition a file of pre-computed hash values for every possible combination of characters. VERY BIG FILE!!!


