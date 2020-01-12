# Bliss Q

![g6](https://github.com/magicxavi/manifest/raw/blissQ-g6/BLISS%20ROM_LG%20G6.png "g6")

Synch sources:

    $ repo init -u https://github.com/BlissRoms/platform_manifest.git -b q
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/blissQ-zuk/bliss.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for LG G6
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch bliss_z2_plus-userdebug
    $ make blissify
