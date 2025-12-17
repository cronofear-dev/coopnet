# Installation guide (Tested in Ubuntu Server 24)
### Install the dependencies
```bash
sudo apt update
sudo apt install build-essential git cmake libssl-dev libcurl4-openssl-dev
```

### Install libjuice dependency
```bash
git clone https://github.com/paullouisageneau/libjuice.git
cd libjuice
cmake -B build
cmake --build build
sudo cmake --install build
```

### Install and run coopnet
```
git clone https://github.com/cronofear-dev/coopnet.git
cd coopnet
make
cd bin
./server
```

`./server` runs the server. The server can be also run as a service background so it can run on system reboot.
