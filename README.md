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

OPENSSL<br>
https://www.openssl.org/
