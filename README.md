= JoBa-VPN

trivial android app that just opens the VPN settings page and quits.
Nice to have a start icon for fast vpn start/stop.

== Instructions

* Download and install Android Studio 3.5 (or probably any other)

 cd
 wget https://dl.google.com/dl/android/studio/ide-zips/3.5.0.21/android-studio-ide-191.5791312-linux.tar.gz
 tar xzf android-studio-ide-191.5791312-linux.tar.gz

* Start Android Studio and download an SDK, e.g. Oreo 8.0

 ~/android-studio/bin/studio.sh

    * Select menu Tools/SDK Manager
    * Select the SDK (e.g. Oreo 8.0)
    * Press OK

This should download all you need to compile and transfer the app to your android phone

* Clone this repo into Android Studio

    * Select menu File/New/Project5 from Version Control/Git
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
        * Enable "OEM Unlock" (not really sure...)
    * Connect phone to USB port (on windows you may need a driver, I used linux)
        * Allow debug access when asked on the phone

* Build and Install
    * Open the project with menu File/Open
    * Toolbar should show hammer icon, then "app" configuration and your phone as target device
    * Select the triangle (or Shift-F10) to build, install and run the app on your phone
