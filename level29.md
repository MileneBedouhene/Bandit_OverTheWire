# Level29 -> Level30

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit29@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "mkdir /tmp/bandit_29"
2. Execute the command "cd /tmp/bandit_29"
3. Execute the command "git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo"
4. Execute the command "git branch -a"
5. Execute the command "git checkout remotes/origin/dev"
6. Execute the command "ls"
7. Execute the command "cat README.md"
8. Output password : qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL