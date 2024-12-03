# Level22 -> Level23

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit22@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "cd  /etc/cron.d/".
2. Execute the command "cat cronjob_bandit23".
3. Execute the command "cat /usr/bin/cronjob_bandit23.sh".
4. Execute the command "cd /usr/bin".
5. Execute the command "./cronjob_bandit23.sh".
6. Execute the command "cat /tmp/8ca319486bfbbc3663ea0fbe81326349"
7. Output password : 0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
