# AEX Nougat

Synch sources:

    $ repo init -u git://github.com/AospExtended/manifest.git -b 7.x
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/aex7.1.2/aex.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch aosp_kenzo-userdebug
    $ mka aex -j$(nproc --all)
