CrookedAndroid

Getting Started To get started with building CrookedAndroid Rom, you'll need to get familiar with Git and Repo.

Setting up the Build Environment: Use this Guide as a reference for getting started

Initialize Source:

mkdir crooked (or whatever you want to name the source folder)

cd ~/crooked

repo init -u https://github.com/CrookedAndroid/manifest.git -b cr2

Sync Source:

repo sync -c -j16 --force-sync --no-clone-bundle --no-tags

Build Source:

. build/envsetup.sh

lunch crooked_devicename-user (device codename)

brunch crooked_devicename-user

