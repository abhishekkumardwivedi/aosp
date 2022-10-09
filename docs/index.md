# Android Containers and file formats

##  APK

* `.apk` : packaging to .apk, from .dex, uses `aapt` tool
  * `.dex` : several .class to single .dex by `dx` tool. Gives better performance compare to old school .jar archieve.
  * `.odex`
  * `.vdex`
  * `.art`
  * `.oat` : tool `dex2oat`. While installing app, ART uses `dex2oat` to compile `.dex` files to `.oat` file.

## Apex

* `.apex` a new contrainer format for low level system modules. [apex](https://android.googlesource.com/platform/system/apex/+/refs/heads/master/docs/README.md) used for hals, art, native libraries and system services. Apex uses apk infrastructure for installation and signing. Additional requrements for apex are `loop driver` and `dm-verity`.
