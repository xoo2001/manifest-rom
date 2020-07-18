# Havoc 3.0 10 Android

Synch sources:

    $ repo init -u https://github.com/Ancient-Lab/manifest -b ten
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/havoc3.0/havoc.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch havoc_kenzo-userdebug
    $ brunch havoc_kenzo-userdebug
