# zen-nomp

Requirements

Currently, you will need:

+ Linux Ubuntu 16.04
+ 64-bit
+ 4GB of free memory(orr swap 4gb)


install ubuntu server and get it updated:

    sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade

Description:

    sudo apt-get install cmake libssl-dev libsodium-dev libpcre3-dev libleveldb-dev libboost-all-dev libgmp-dev libprotobuf-dev protobuf-compiler libjansson-dev screen build-essential pkg-config libc6-dev m4 g++-multilib autoconf libtool ncurses-dev unzip git python zlib1g-dev wget bsdmainutils automake npm redis-server 
  
    sudo npm install n -g

    sudo n stable
  
Download sources:

    git clone https://github.com/zencashio/zen.git zencin

    git clone https://github.com/norens/zen-nomp.git nomp-zen

Build coin sources:

    cd zencoin/
    & ./zcutil/build.sh -j$(nproc)
    & ./zcutil/fetch-params.sh
  
    nano /home/zen/.zen/zen.conf
  
    testnet=0
    addnode=69.164.218.197
    addnode=10.0.0.2:8233
    server=1
    rpcuser=you_user
    rpcpassword=you_pass
    rpcport=8232
    rpcconnect=127.0.0.1
    
Start daemon 

    ./src/zend 
    ./src/zend -daemon
    
Generate wallet addres

    ./src/zen-cli getnewaddress

and

     ./src/zen-cli z_getnewaddress
     
More command https://github.com/zcash/zcash/blob/v1.0.1/doc/payment-api.md
  
Build pool sources:
  
    cd nomp-zen
  
    npm update
    
    npm install

    sudo service redis-server restart
    
Config you web-site
    
    nano config.json

Say you wallet addres in pool-config
    
    
    nano pool_configs/zen.conf

Start pool

    cd nomp-zen
    
    npm start


Miner connect in 3357 port  


Donate

+Bitcoin 3Jtuqsq5pEkWiFCp3yThmAvCM2q5y51tyS
+Zcash t1bjfQmQkfFs39gpeEPCV55SQ7YyuW1qmYL
+Zen t1azCzJxSoWCrZkzg35BpKnmVE6BnfVECnT

