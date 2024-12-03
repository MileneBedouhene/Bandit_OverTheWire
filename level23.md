# Level23 -> Level24

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit23@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the command "cd /etc/cron.d".
2. Execute the command "ls".
3. Execute the command "cat cron".
4. Execute the command "cat cronjob_bandit24".
4. Execute the command "cat /usr/bin/cronjob_bandit24.sh".
4. Execute the command "cd /var/spool/bandit24/foo"
4. Execute the command "nano get.sh"
4. Execute the command "chmod +x get.sh"
4. Execute the command "cat /tmp/pass/password.txt"
5. Output password :  gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8
