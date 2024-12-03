# Level25 -> Level26

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit25@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "ls"
2. Execute the command "cat bandit26.sshkey"
3. Execute the command "cat /etc/passwd | grep bandit26"
4. Reduce the size of the terminal window
5. Execute the command "ssh -t -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220"
6. Press "v"
7. Write ":e /etc/bandit_pass/bandit25"
8. Output password : s0773xxkk0MXfdqOfPRVr9L3jJBUOgCZ
9. Write ":set shell?"
10. Write ":set shell=/bin/bash"
11. Write ":shell", to move to bandit26