# Password-Manager
Objective:
Design a program that keeps track of all passwords provided to all website accounts while maintaining security.


Method:
  The program will implement the use of a random character generator to create a 16 character password. The intent is to use this password for only one account in order to avoid repetition of passwords. Failure to do so could increase the probability of an attacker being able to break into 2 different accounts.

  In order to keep track of the passwords for the user, all passwords will be copied into a text file. When the user wishes to enter an account, the user will need to access this document to find the password for the respective website. To do this, the text file must be uploaded to a cloud server for easier access.
  
  In order to protect the user's information, a master password must be chosen for the cloud server account. This password will not be composed of random characters; rather, it will be chosen by using Diceware. More information can be found at https://www.rempe.us/diceware/#diceware
  

Password Details:
  The password generated for all websites (except the cloud server) will be random. There are 96 unique characters in the standard QWERTY keyboard (26 uppercase letters, 26 lowercase letters, 10 numbers, and 34 symbols including whitespace)
  
  By using this method, the password will have high security since Brute Force will take at most 96^16 attempts to guess it correctly. Dictionary attacks will be ineffective as well due to the randomness of the password. 
  
  Only strings will be generated, the respective website will handle extra security through hashing and/or salting.

  
Master Password Details:
  This password must be remembered by the user. It must be extremely strong but easy to remember. Diceware will be the most reliable method for choosing this password as the nature of it protects ot from both Brute Force and Dictionary Attacks.
  
  Simply put, Diceware uses a list of 7,776 carefully chosen words and chooses 5 words (or more, depending on the user) by using the result of 5 consecutive and unbiased dice rolls.
  
  More words will undoubetdly increase the security of the passwords, but
