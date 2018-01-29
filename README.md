Hsrminer neoscrypt fork by Justaminer, version 29.01.2018

Features:

~    0% devfee

~    added options --api-bind, --algo, -a, --benchmark, --retries , see --help for details

~    API is working! By default you can connect to 127.0.0.1:4068 from the same computer. 

~    Option -b ip:port added to control API, usage example:

     -b 0.0.0.0 will allow to connect from external hosts, for now you can control access via firewall, option --api-allow will be added later
     
     -b 0 will disable API.

~    -r N option added, where N is number of reconnect attempts, usage example:
     
     hsrminer_neoscrypt_fork.exe -r 1 -o URL -u User -p Pass 
     
     This option will make miner try to reconnect 1 time if connection to pool failed and then exit.
    
     If you specify -r 0 , miner will exit immediately after connection to pool lost.
