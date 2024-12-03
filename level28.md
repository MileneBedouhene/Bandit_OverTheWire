# Level28 -> Level29

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit28@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "mkdir /tmp/bandit_28"
2. Execute the command "cd /tmp/bandit_28"
3. Execute the command "git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo"
4. Execute the command "ls"
5. Execute the command "cd repo"
6. Execute the command "git log"
7. Execute the command "git checkout 73f5d0435070c8922da12177dc93f40b2285e22a"
8. Execute the command "cat README"
9. Output password : 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7