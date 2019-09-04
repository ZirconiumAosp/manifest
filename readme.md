<img src="https://raw.githubusercontent.com/ZirconiumAosp/manifest/q/zircon.png"> 

ZirconiumAosp
=========

Credits 
-------
 * [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
 * [**POSP**](https://github.com/PotatoProject-next)

Getting Started 
--------------- 
To get started with the ZirconiumAosp sources, you'll need to get 
familiar with [Git and Repo](https://source.android.com/setup/develop.html). 

Use corona-release branch for Android Pie and pulsar-release branch for Android Oreo.

Initialize the Repositories 
---------------------------

    repo init -u https://github.com/ZirconiumAosp/manifest.git -b q

    repo sync --force-sync -c --no-tags --no-clone-bundle -jX

 -j# -Set jobs by just replacing # with what you wish

This will initialize the new repository and begin the initial sync. This can take a while!

Building the System 
-------------------
 Initialize the ROM environment with the envsetup.sh script. By entering command (i).

     . build/envsetup.sh
     lunch zirconium_<device>-userdebug
     make otapackage 
