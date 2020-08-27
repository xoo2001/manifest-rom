# Ancient Civilization 10 Android

![Xiaomi Redmi Note 3](https://github.com/magicxavi/manifest/raw/ancientQ/PicsArt_07-15-12.05.11.png "Xiaomi Redmi Note 3")

Synch sources:

    $ repo init -u https://github.com/Ancient-Lab/manifest -b ten
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/ancientQ/ancient.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch ancient_kenzo-userdebug
    $ mka bacon -j$(nproc --all)
