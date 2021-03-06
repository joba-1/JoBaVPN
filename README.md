# JoBa-VPN

trivial android app that just opens the VPN settings page and quits.
Nice to have a start icon for fast vpn start/stop.

## Instructions

I did that on linux, so you may adapt things for other OS

* Download and install Android Studio 3.5 (or probably any other)
```
cd
wget https://dl.google.com/dl/android/studio/ide-zips/3.5.0.21/android-studio-ide-191.5791312-linux.tar.gz
tar xzf android-studio-ide-191.5791312-linux.tar.gz
```
* Start Android Studio
```
~/android-studio/bin/studio.sh
```
* Download an SDK
    * Select menu Tools/SDK Manager (or studio offers latest sdk installation on first start) 
    * Select the SDK (e.g. Oreo 8.0)
    * Press OK
 
This should download all you need to compile and transfer the app to your android phone

* Clone this repo into Android Studio

    * Select menu File/New/Project from Version Control/Git (or studio offers this option at first start)
    * Enter repo URL https://github.com/joba-1/JoBaVPN
    * Select Clone

* Prepare the phone

    * Enable Developer Menu (only needed once)
        * Go to Settings/Phone Info/Software Information
        * Tap on Build Number seven times
    * Enable USB Debugging
        * Go to menu Settings/Developer Options
        * Switch them on
        * Enable "Stay awake"
        * Enable "USB Debugging"
    * Connect phone to USB port
        * Allow debug access when asked on the phone

* Build and Install
    * Open the project with menu File/Open (or it is already open after first clone)
    * Toolbar should show hammer (build) icon, then "app" configuration and your phone as target device
    * Select the triangle (or Shift-F10) to build, install and run the app on your phone

## Details

* The project is based on the "Empty Activity" new project template.
* Basically all I changed was [MainActivity.kt line 13-16](../master/app/src/main/java/com/joba/vpn/MainActivity.kt#L13)
* Should work with any android phone and version
* Tested with 
    * Samsung S5 mini / Android 6 / SDK 10.0 API 29
    * Samsung S7 / Android 8 / SDK 8.0 API 26
