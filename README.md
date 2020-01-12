# Bliss Q

![Xiaomi Redmi Note 3](https://github.com/magicxavi/manifest/raw/blissQ/BLISS%20ROM_Xiaomi%20Redmi%20Note%203%20(2).png "Xiaomi Redmi Note 3")

Synch sources:

    $ repo init -u https://github.com/BlissRoms/platform_manifest.git -b q
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/blissQ/bliss.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch bliss_kenzo-userdebug
    $ make blissify
