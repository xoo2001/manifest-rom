# Havoc 3.x 10 Android

![Lenovo A6000](https://github.com/magicxavi/manifest/raw/havoc/photo_2020-04-25_02-48-40.jpg "Xiaomi Redmi Note 3")

Synch sources:

    $ repo init -u git://github.com/crdroidandroid/android.git -b 10.0
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/xoo2001/manifest-rom/lineage/lineage.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Lenovo A6000
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch lineage_a6000-userdebug
    $ brunch lineage_a6000-userdebug
