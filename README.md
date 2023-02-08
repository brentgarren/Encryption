# Encryption

GNU Privacy Guard for Encryption<br>
gpg --symmetric --cipher-algo CIPHER message.txt, where "CIPHER=encryption algorithm" You can see a list of encryption methods via "gpg --version"

-----------------------

GNU Privacy Guard for Decryption <br>
gpg --output original_message.txt --decrypt message.gpg

--example<br>
  gpg --output mymessage.txt --decrypt mymessage.gpg
