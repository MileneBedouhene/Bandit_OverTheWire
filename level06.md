# Level6 -> Level7

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit6@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "find / -type f -size 33c -user bandit7 -group bandit6 2>/dev/null", to search for 33 byte files belonging to bandit7 and the bandit6 group, ignoring permission errors.
2. After finding the file execute the command "cat /var/lib/dpkg/info/bandit7.password", 
4. Output password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj