# Bliss Q

![MI A3](https://github.com/magicxavi/manifest/raw/blissQ-laurel/BLISS%20ROM_Xiaomi_Mi_A3.png "MI A3")

Synch sources:

    $ repo init -u https://github.com/BlissRoms/platform_manifest.git -b q
    $ mkdir -p .repo/local_manifests
    $ wget https://github.com/magicxavi/manifest/raw/blissQ-laurel/bliss.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi MI A3 (laurel_sprout)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch bliss_laurel_sprout-userdebug
    $ make blissify
