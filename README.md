VM13 by Team Nocturnal
Download the source

Please read the VM13 building instructions before proceeding.

Initialize:

Create the build directory :

$ mkdir ~/dev
$ mkdir ~/dev/vm13
$ cd ~/dev/vm13
Init core trees without any device/kernel/vendor :

$ repo init -u https://github.com/VM13/platform_manifest.git -b vm13

$ repo sync

Start Building

After the sync is finished, please read the instructions from the Android site on how to build.

. build/envsetup.sh
brunch
make -j8
You can also build (and see how long it took) for specific devices like this:

. build/envsetup.sh
time brunch vm13_shamu-userdebug
make -j8
Remember to make clobber every now and then!
