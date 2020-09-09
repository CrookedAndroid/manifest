Franken

Getting Started
To get started with building Franken Rom, you'll need to get familiar with Git and Repo.

Setting up the Build Environment: Use this Guide as a reference for getting started

Initialize Source:

    mkdir franken (or whatever you want to name the source folder)

    cd ~/franken
    repo init -u https://github.com/FrankenRom11/manifest.git -b fr-11
Sync Source:

    repo sync -c -j16 --force-sync --no-clone-bundle --no-tags
Build Source:

    . build/envsetup.sh
    lunch franken_devicename-userdebug (device codename)
    make clean
    make franken
