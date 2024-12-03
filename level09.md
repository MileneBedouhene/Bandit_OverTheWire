# Level9 -> Level10

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit9@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "strings data.txt | grep '=*', to find all printable strings in data.txt and filter out those that contain equal signs.
2. Output password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey