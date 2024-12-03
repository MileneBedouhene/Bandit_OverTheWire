# Level12 -> Level13

### Steps :
-  Connecting to the game using the command:
    
    ssh bandit12@bandit.labs.overthewire.org -p 2220


-  to find the level password which was stored in a personal directory:
1. Execute the command "TEMP_DIR=$(mktemp -d)", to create a tmp folder.
2. Execute the command "cd $TEMP_DIR",to access the tmp folder.
3. Execute the command "nano decompress.sh", to create a script bash.
decompress.sh:
'''

#!/bin/bash

cp ~/data.txt 

xxd -r data.txt data.bin

    while true; do

        file_type=$(file -b data.bin)  

        echo "Type de fichier: $file_type"
    
        if [[ $file_type == *"gzip compressed data"* ]]; then
            mv data.bin data.bin.gz
            gunzip data.bin.gz
        elif [[ $file_type == *"bzip2 compressed data"* ]]; then
            mv data.bin data.bin.bz2
            bunzip2 data.bin.bz2
        elif [[ $file_type == *"XZ compressed data"* ]]; then
            mv data.bin data.bin.xz
            unxz data.bin.xz
        elif [[ $file_type == *"POSIX tar archive"* ]]; then
            mv data.bin data.bin.tar
            tar -xf data.bin.tar
            data_bin_new=$(ls -1 | grep -v 'data.txt' | head -n 1)  # Trouver le nouveau fichier
            if [[ -z $data_bin_new ]]; then
                echo "Aucun nouveau fichier trouvé après extraction tar."
                break
            fi
            mv "$data_bin_new" data.bin  # Renommer le fichier extrait pour la prochaine itération
        elif [[ $file_type == *"ASCII text"* ]]; then
            cat data.bin  # Afficher le contenu du fichier texte
            break
        else
            echo "Type de fichier inconnu: $file_type"
            break
        fi
    done
'''
4. Execute the command "chmod +x decompress.sh", to be able to execute the script.
5. Output password: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn