# Encryption

GNU Privacy Guard for Encryption<br>
https://gnupg.org/<br>
gpg --symmetric --cipher-algo CIPHER message.txt, <br>
where "CIPHER=encryption algorithm" <br>
You can see a list of encryption methods via "gpg --version"

-----------------------

GNU Privacy Guard for Decryption <br>
gpg --output original_message.txt --decrypt message.gpg

--example<br>
  ![decrypt](https://user-images.githubusercontent.com/105601437/217442653-b0ce251d-76c9-4dff-8bd9-d65e2484e60a.png) <br>


-------------------
OPENSSL for Encryption
https://www.openssl.org/ <br>

openssl aes-256-cbc -e -in message.txt -out encrypted_message

-------------------

OPENSSL for Decryption
openssl aes-256-cbc -d -in encrypted_message -out original_message.txt

-------------------
To make the encryption more secure and resilient against brute-force attacks, we can add -pbkdf2 to use the Password-Based Key Derivation Function 2 (PBKDF2); moreover, we can specify the number of iterations on the password to derive the encryption key using -iter NUMBER. To iterate 10,000 times, the previous command would become:

Encryption

openssl aes-256-cbc -pbkdf2 -iter 10000 -e -in message.txt -out encrypted_message

Decryption

openssl aes-256-cbc -pbkdf2 -iter 10000 -d -in encrypted_message -out original_message.txt

------------------
