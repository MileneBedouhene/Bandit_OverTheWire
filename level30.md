# Level30 -> Level31

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit30@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "mkdir /tmp/bandit_30"
2. Execute the command "cd /tmp/bandit_30"
3. Execute the command "git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo"
4. Execute the command "cd repo"
5. Execute the command "git config --local --add safe.directory $(pwd)"
6. Execute the command "git tag"
7.Execute the command "git show secret"
8. Output password : fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy