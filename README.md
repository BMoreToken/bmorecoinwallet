[![Nightly Build](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/nightly.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/nightly.yml) 
[![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/BMoreToken/bmorecoinwallet.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/BMoreToken/bmorecoinwallet/context:cpp)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/BMoreToken/bmorecoinwallet.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/BMoreToken/bmorecoinwallet/alerts/)
[![CodeQL](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/codeql-analysis.yml)

# Ubuntu 18.04
[![Ubuntu 18.04](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/ubuntu18.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/ubuntu18.yml)
* sudo apt install -y qt5-default qttools5-dev qttools5-dev-tools libqt5charts5-dev libboost1.65-all-dev

# Ubuntu 20.04
[![Ubuntu 20.04](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/ubuntu20.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/ubuntu20.yml)
* sudo apt install -y qt5-default qttools5-dev qttools5-dev-tools libqt5charts5-dev libboost1.67-all-dev

# AppImage
[![AppImage](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/appimage.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/appimage.yml)
* sudo apt install -y qt5-default qttools5-dev qttools5-dev-tools libqt5charts5-dev libboost1.65-all-dev

# Windows
[![Windows Nightly](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/Windows_nightly.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/Windows_nightly.yml)
[![Windows](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/windows.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/windows.yml)

# macOS
[![macOS Nightly](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/macOS_nightly.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/macOS_nightly.yml)
[![macOS](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/macOS.yml/badge.svg)](https://github.com/BMoreToken/bmorecoinwallet/actions/workflows/macOS.yml)


# How to get BALTx - Ubuntu
## Do this once to install
* cd ~
* wget https://github.com/xmrig/xmrig/releases/download/v6.16.2/xmrig-6.16.2-linux-x64.tar.gz
* tar -xvf xmrig-6.16.2-linux-x64.tar.gz
* sudo mv xmrig-6.16.2/xmrig /bin/xmrig
* git clone https://gist.github.com/73362a23ccbb1aeb7bea9a1e50a52cba.git sample
* cp sample/config.json config.json
* REPLACE user WITH YOUR NEW WALLET ADDRESS IN config.json
## Do this to start making BALTx
* xmrig -c config.json 
* View your status at https://pool.bmorecoin.com/#worker_stats


# Old instructions for Windows 11/10: Use Ubuntu for Windows
## Ubuntu for Windows
* https://www.microsoft.com/en-us/p/ubuntu/9nblggh4msv6
* Open in "Store" and install
## WSL
* https://docs.microsoft.com/en-us/windows/wsl/install
* run Powershell "as Admin" to install wsl
<pre>
wsl --install
</pre>
* Reboot PC


# Ubuntu / Linux
* 1: sudo apt update
* 2: sudo apt upgrade
* 3: sudo apt install git gcc make cmake libboost1.67-dev qt5-default build-essential
* 4: git clone https://github.com/BMoreToken/bmorecoinwallet
* 5 : cd bmorecoinwallet
* 6: git clone https://github.com/BMoreToken/bmorecoin cryptonote
* 7: mkdir build; cd build
* 8: cmake ..
* 9: make
* 10: ./bmorecoin &

*
