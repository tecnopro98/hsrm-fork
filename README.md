Hsrminer neoscrypt fork by Justaminer, version 08.02.2018

Features:

~    0% devfee

     Version: 08.02.2018

~    fixed palgin's bug in -d option parsing, so now you can use -d with card's number > 9, i.e. -d 10,11,12. This miner supports up to 16 gpus( from 0 to 15 in -d parameter).

~    API now correctly shows GPU's core frequency, fan %, temperature and hashrate for each gpu, also total accepted/rejected counters.

~    Added separate high process priority version (hsrminer_neoscrypt_fork_hp.exe) which will give more hashrate (I get +50 kh/s for 1070), but it will stress GPUs more, so overclocked too much GPU's can crash\hang, etc. So if you have troubles with this version, use normal process priority version (hsrminer_neoscrypt_fork.exe).

     Version: 31.01.2018

~    fixed crash on Windows 10 1709

~    added options --api-bind, --algo, -a, --benchmark, --retries , see --help for details

~    API is working! By default you can connect to 127.0.0.1:4068 from the same computer. 

~    Option -b ip:port added to control API, usage example:

     -b 0.0.0.0 will allow to connect from external hosts, for now you can control access via firewall, option --api-allow will be added later
     
     -b 0 will disable API.

~    -r N option added, where N is number of reconnect attempts, usage example:
     
     hsrminer_neoscrypt_fork.exe -r 1 -o URL -u User -p Pass 
     
     This option will make miner try to reconnect 1 time if connection to pool failed and then exit.
    
     If you specify -r 0 , miner will exit immediately after connection to pool lost.
