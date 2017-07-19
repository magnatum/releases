# releases
Wallets and Essentials <br><br>
Signatum releases for Windows, Linux, ARM and more.<br>
<br>
Instructions for Linux Qt depends.<br>
------------------------------------<br>

If you get dependencies errors then it means you are missing one of these: <br>
libssl-dev libdb++-dev libdb-dev libboost-all-dev libqrencode-dev libminiupnpc-dev <br>
Install by sudo apt-get install libssl-dev libdb++-dev libdb-dev libboost-all-dev libqrencode-dev libminiupnpc-dev <br>
<br>
Contributed by Itamar Carvalho for Arch Linux <br><br>
First of all we need to install the dependencies, if you miss something<br>
sudo pacman -S boost-libs desktop-file-utils libevent miniupnpc protobuf qrencode qt5-base zeromq<br>
Then we need to link the old version that signatum asks for the newest version that we have installed<br>
sudo ln -sf /usr/lib/libminiupnpc.so.16 /usr/lib/libminiupnpc.so.10<br>
sudo ln -sf /usr/lib/libboost_system.so.1.64.0 /usr/lib/libboost_system.so.1.58.0<br>
sudo ln -sf /usr/lib/libboost_filesystem.so.1.64.0 /usr/lib/libboost_filesystem.so.1.58.0<br>
sudo ln -sf /usr/lib/libboost_program_options.so.1.64.0 /usr/lib/libboost_program_options.so.1.58.0<br>
sudo ln -sf /usr/lib/libboost_thread.so.1.64.0 /usr/lib/libboost_thread.so.1.58.0 <br>
