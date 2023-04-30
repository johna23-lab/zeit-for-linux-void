# Zeit project
 Qt frontend to `crontab` and `at`

### Features: ###
* Add, edit and delete `crontab` tasks
* Add, edit and delete environment variables for `crontab`
* Add and delete `at` commands
* Alarms and Timers
* Optional root actions, PolKit support (KF5Auth and KF5CoreAddons needed)

### How to install in Linux Void

wget https://github.com/johna23-lab/zeit-for-linux-void/releases/download/de6b5c2_1/zeit-de6b5c2_1.x86_64.xbps

xbps-rindex -a zeit-de6b5c2_1.x86_64.xbps

sudo xbps-install -R $PWD zeit-de6b5c2_1


### Build dependencies ### (For debian)
Extra CMake Modules, QtBase, QtTools, KF5Auth (optional), KF5CoreAddons (optional)

```bash
sudo apt install qtbase5-dev qttools5-dev libkf5auth-dev libkf5coreaddons-dev extra-cmake-modules
```

### Runtime dependencies ###
libnotify-bin, mpv

### Build and run ###
```bash
mkdir build && cd build
cmake ..
make -j2
./src/zeit
```

### Screenshot ###
![Screenshot of the Zeit app](https://raw.githubusercontent.com/loimu/zeit/master/assets/screenshot.png)

### Installation on Ubuntu ###
```bash
# stable releases
sudo add-apt-repository ppa:blaze/main
sudo apt update
sudo apt install zeit

# development snapshots
sudo add-apt-repository ppa:blaze/dev
sudo apt update
sudo apt install zeit
```
