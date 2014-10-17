NamelessROM for the Huawei Y300
===============================

Local Manifest to build NamelessROM for the Huawei Y300

Build Instructions for NamelessROM Y300 (U8833)
-----------------------------------------------------------------------------

1. Initialize repo using the NamelessROM manifest

        repo init -u https://github.com/NamelessRom/android.git -b android-4.4

2. Add my local manifest

        mkdir .repo/local_manifests
        curl https://raw.githubusercontent.com/NamelessRomY300/android/master/nameless_huawei.xml > .repo/local_manifests/nameless_huawei.xml

3. Then sync up the repositories
 
        repo sync -f -j8

4. Initialize the build environment

        source build/envsetup.sh
    
5. Build the ROM

        For Y300:
            brunch u8833
