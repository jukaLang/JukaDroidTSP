# JukaDroidTSP

An Android Operating System for Trimui Smart Pro.

Please consider contributing to the source!

## Development Instructions

- Install git openjdk-11-jdk python3 repo
- Clone this repository, "git clone https://github.com/jukaLang/jukaDroidTSP"
- Initialize repo (setup main android source) "repo init -u https://android.googlesource.com/platform/manifest"   and then do "repo sync" (may take hours)
- Clone all winner kernel, "git clone https://github.com/allwinner-dev-team/linux-allwinner.git -b allwinner-3.0"


TODO:
- Add Kernel Source
- Create or find a device tree for TSP


- Run "source build/envsetup.sh"
- "lunch aosp_arm64-eng"
- Compile code "make -j$(nproc)"  <- will take many many hours.


Flash Images:
- fastboot flash boot boot.img
- fastboot flash system system.img
- fastboot flash userdata userdata.img
- fastboot flash recovery recovery.img
- fastboot reboot