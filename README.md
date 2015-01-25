SimpleAOSP Github
===================

Setting up your Build Environment
---------------------------------
- Official build environment as per Google and AOSP [Android source page](http://source.android.com/source/index.html)
- XDA user guides [Ubuntu 14.04 Trusty LTS](http://forum.xda-developers.com/showthread.php?t=2639611) , [Ubuntu 14.10 Utopic](http://forum.xda-developers.com/chef-central/android/howto-setup-ubuntu-14-10-utopic-unicorn-t2862442)
- Arch Linux(https://wiki.archlinux.org/index.php/android#Building_Android)

Initializing the Source
-----------------------
(Assuming you have a valid build environment set up)
- mkdir simpleaosp
- cd ~/simpleaosp
- repo init -u https://github.com/SimpleAOSP-Lollipop/platform_manifest.git -b L

Syncing the Source
---------------
- repo sync -jx -f (x being the number of CPU jobs)

Getting Ready to Build
----------------------
- . build/envsetup.sh

Choose Any Among the Supported Devices to Build
-----------------------------------------------
- lunch simpleaosp_flo-user 
- lunch simpleaosp_flounder-user
- lunch simpleaosp_hammerhead-user
- lunch simpleaosp_mako-user
- lunch simpleaosp_shamu-user

Now Build it
------------
- mka otapackage

For Quick Dirty Rebuilds
------------------------
- cd ~/simpleaosp
- repo sync -jx -f (x being the number of CPU jobs)
- lunch and pick the right device (refer the list above for supported devices)
- mka dirty
- mka otapackage

Credits
-------
- Google for AOSP
- Rascarlo and RastaPop
- Altaf-Mahdi and Euphoria-OS
- DariosF and Purity ROM
- Paranoid Android (AOSPA)
- AOSPAL
- CyanogenMod
- Dirty Unicorns
- LiquidSmooth
- AOKP
- SlimROMS
- Project D.I.S.C.O. Team
- PartimusPrime for boot-animations
- OmniROM
- Lichti1901 and Terminus
- Sykopompos
- Team Horizon and XenonHD
- Chet and OptiPop
- VanirAOSP
- PurifiedROM
- The-Ancile-Project
- AOD-Lollibeans
- Android Open Development
- Dhacker29
- beanstown106
- Ayysir
- Others we may have missed
