# Level18 -> Level19

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit18@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "ssh -t bandit18@bandit.labs.overthewire.org -p 2220 /bin/sh "to bypass issues with .bashrc and start a shell session on port 2220, allowing you to access the readme file and retrieve the next password.
2. Execute the command "cat readme". 
3. Output password : cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8