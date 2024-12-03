# Level5 -> Level6

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit5@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "cd ./inhere" to access the folder.
2. Execute the command "find . -type f -size 1033c -exec file {} + | grep 'text'",to select file which has a size of 1033 bytes and which is human readable in all directories and subdirectories, to get all the file information and keep only those which are human readable.
3. After finding the file execute the command "cat ./maybehere07/.file2", 
4. Output password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG