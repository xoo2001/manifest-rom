# local_manifest for LiquidRemix Kenzo

Synch sources:

    $ repo init -u git://github.com/LiquidRemix/android_manifest.git -b pie
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/local_manifest_LiquidRemix/master/liquid.xml -O .repo/local_manifests/liquid.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch liquid_kenzo-userdebug
    $ brunch liquid_kenzo-userdebug
