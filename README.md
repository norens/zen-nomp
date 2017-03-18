# zen-nomp
install ubuntu server and get it updated:

sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade

Description

sudo apt-get install cmake libssl-dev libsodium-dev libpcre3-dev libleveldb-dev libboost-all-dev libgmp-dev libprotobuf-dev protobuf-compiler libjansson-dev screen build-essential pkg-config libc6-dev m4 g++-multilib autoconf libtool ncurses-dev unzip git python zlib1g-dev wget bsdmainutils automake npm redis-server 
  
sudo npm install n -g
sudo n stable
  
  Download sources
git clone https://github.com/zencashio/zen.git zencin
git clone https://github.com/norens/zen-nomp.git nomp-zen

Build pool sources
cd zencoin/
./zcutil/build.sh -j$(nproc)
./zcutil/fetch-params.sh
