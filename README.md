# Havoc 3.x 10 Android

![Xiaomi Redmi Note 3](https://github.com/magicxavi/manifest/raw/havoc/photo_2020-04-25_02-48-40.jpg "Xiaomi Redmi Note 3")

Synch sources:

    $ repo init -u https://github.com/Havoc-OS/android_manifest.git -b ten
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/havoc/havoc.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch havoc_kenzo-userdebug
    $ brunch havoc_kenzo-userdebug
