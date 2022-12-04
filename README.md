# motoG5

* https://motorola-global-portal.custhelp.com/app/standalone/bootloader/unlock-your-device-b
* https://wiki.lineageos.org/devices/cedric/install
* https://lineageosroms.com/cedric/
* https://download.lineageos.org/cedric
* https://mirrorbits.lineageos.org/full/cedric/20221115/lineage-18.1-20221115-nightly-cedric-signed.zip
* https://mirrorbits.lineageos.org/full/cedric/20221115/lineage-18.1-20221115-nightly-cedric-signed.zip?sha256
* https://mirrorbits.lineageos.org/recovery/cedric/20221115/lineage-18.1-20221115-recovery-cedric.img
* https://mirrorbits.lineageos.org/recovery/cedric/20221115/lineage-18.1-20221115-recovery-cedric.img?sha256
* https://motorola-global-portal.custhelp.com/euf/assets/downloads/Motorola_Mobile_Drivers_64bit.msi
* https://android-sdk-tools.en.lo4d.com/download/mirror-ls1

# install
## install recovery image
fastboot flash recovery lineage-18.1-20221115-recovery-cedric.img

## install lineage os
adb sideload lineage-18.1-20221115-nightly-cedric-signed.zip

# troubleshooting

## "oem unlock" is not allowed  
- Enable developper mode.
- Insert a SIM card into Moto G5
 and try again.
 
## ERROR: This package requires firmware from an Adroid 8.1 based stock ROM build. Please upgrade firmware and retry!
Download [stock rom](https://mirrors-obs-2.lolinet.com/firmware/motorola/2017/cedric/official/RETAIL/CEDRIC_RETAIL_8.1.0_OPP28.85-19-4-2_cid50_subsidy-DEFAULT_regulatory-DEFAULT_CFC.xml.zip) and make modem newer. 

Extract the zip file. This zip includes NON-HLOS.bin.

fastboot flash modem NON-HLOS.bin



