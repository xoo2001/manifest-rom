# LiquidRemix Pie

Synch sources:

    $ repo init -u https://github.com/BlissRoms/platform_manifest.git -b p9.0
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/bliss/bliss.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch bliss_kenzo-userdebug
    $ make -j$(nproc --all) Blissify
