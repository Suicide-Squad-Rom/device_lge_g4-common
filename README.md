Copyright 2015 - The CyanogenMod Project

Device configuration for LG G4.
=====================================

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Dual-core 2.0 GHz ARM® Cortex™ A57 and quad-core 1.5 GHz ARM® Cortex™ A53
CHIPSET | Qualcomm MSM8992 Snapdragon 808
GPU     | Adreno 418
Memory  | 3GB
Shipped Android Version | 5.1
Storage | 32GB
MicroSD | Up to 128GB
Battery | 3000 mAh
Dimensions | 148.9 x 76.1 x 6.3 - 9.8 mm
Display | 2560 x 1440 pixels, 5.5" HD-IPS LCD
Rear Camera  | 16 MP hybrid infared autofocus, dual-LED flash
Front Camera | 8 MP
Release Date | April 2015

![LG G4](http://cdn2.gsmarena.com/vv/pics/lg/lg-g4-1.jpg "LG G4")


## Device Handler
This is Slim Roms Device Handler

Add the following to enable it for your device

To device.mk

PRODUCT_PACKAGES += \ DeviceHandler

and To overlay/frameworks/base/core/res/res/values/config.xml add:

<!-- The list absolute paths of jar/apk files containing the device specific handlers,
     delimited by File.pathSeparator, which defaults to ":" on Android -->
<string name="config_deviceKeyHandlerLib" translatable="false">/system/app/DeviceHandler.apk</string>

<!-- Full qualified name of the class that implements
     com.android.internal.os.DeviceKeyHandler interface. -->
<string name="config_deviceKeyHandlerClass" translatable="false">com.broken.device.KeyHandler</string>
