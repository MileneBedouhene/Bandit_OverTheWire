# Level31 -> Level32

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit31@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "mkdir /tmp/bandit_31"
2. Execute the command "cd /tmp/bandit_31"
3. Execute the command "git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo"
4. Execute the command "ls"
5. Execute the command "cd repo"
6. Execute the command "ls"
7. Execute the command "cat README.md"
8. Execute the command "echo 'May I come in?' > key.txt"
9. Execute the commande "git add -f ket.txt"
10. Execute the command "git commit -m 'Upload a file'"
11. Execute the command "git push -u origin master"
12. Output password : 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K