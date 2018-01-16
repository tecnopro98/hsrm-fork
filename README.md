Hsrminer neoscrypt fork by Justaminer.

Features:

~   0% devfee

~   -r N option added, where N is number of reconnect attempts, usage example:
     
     hsrminer_neoscrypt_fork.exe -r 1 -o URL -u User -p Pass 
     
     This option will make miner try to reconnect 1 time if connection to pool failed and then exit.
    
     If you specify -r 0 , miner will exit immediately after connection to pool lost.
