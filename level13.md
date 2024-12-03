# Level13 -> Level14

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit13@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "ls", to know what the directory contains.
2. Execute the command "cat bandit14_key",to know the contents of the file(it contains a private RSA key).
3. Execute the command "chmod 600 bandit14_key", to change file permissions.
4. Execute the command "ssh -i bandit14_key -p 2220 -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no bandit14@localhost",
 to allow connecting to the SSH server using the private key bandit14_key and some options to handle host checks.
