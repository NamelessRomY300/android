NamelessROM for the Huawei Y300/G510/G330
=========================================

Local Manifest to build NamelessROM for the Huawei Y300/G510/G330

Build Instructions for NamelessROM
----------------------------------

1. Initialize repo using the NamelessROM manifest
```bash
repo init -u https://github.com/NamelessRom/android.git -b android-4.4
```
2. Add my local manifest
```bash
curl --create-dirs -L -o .repo/local_manifests/roomservice.xml -O -L https://raw.github.com/NamelessRomY300/android/master/nameless_huawei.xml
```
3. Then sync up the repositories
```bash
repo sync -f -j8
```
4. Initialize the build environment
```bash
. build/envsetup.sh
```    
5. Build the ROM
```bash
For Y300:
    brunch u8833
For G510:
    brunch u8951
For G330
    brunch u8825
```
