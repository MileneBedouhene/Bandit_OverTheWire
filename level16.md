# Level16 -> Level17

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit16@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "nmap -p 31000-32000 localhost", to find open ports.
2. Execute the command "openssl s_client -connect localhost:<port>", to check if the port supports SSL/TLS.
3. After finding the port, execute the command "ncat --ssl localhost <port>" and enter the password : kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx,
as a result there will be an rsa encryption key, do an exit and put the key in a file "pvt.key".
4. Execute the command "ssh -i pvt.key bandit17@bandit.labs.overthewire.org -p 2220"
5. Welcome to bandit17
6. Execute the command "cat /etc/bandit_pass/bandit17", to know the password.
7. Output password : EReVavePLFHtFlFsjn3hyzMlvSuSAcRD



