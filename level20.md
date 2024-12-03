# Level20 -> Level21

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit20@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "nc -l -p 12345 < /etc/bandit_pass/bandit20".
2. Execute the command "./suconnect 12345", in another terminal.
3. Output password : EeoULMCra2q0dSkYj561DX7s1CpBuOBt