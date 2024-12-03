# Level15 -> Level16

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit15@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "cat /etc/bandit_pass/bandit15 | openssl s_client -quiet -connect localhost:30001".
2. Output password: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx 