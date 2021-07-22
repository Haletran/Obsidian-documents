# Remove bloat from your Android

In our time, Android phone came with preinstalled apps that you can't remove directly on your smart phone. These apps can be really intrusive  and not very useful. 

So I'm going to show you how to remove these thanks to the help of ADB (Android debug Bridge) which is a tool made by Google for developers. 

## Installation 

So first of all you need to install ADB on your PC , through this link [Android SDK](https://dl.google.com/android/repository/platform-tools-latest-windows.zip). 

Extract the binaries. 

https://www.xda-developers.com/install-adb-windows-macos-linux/

> pm uninstall --user 0 "package name"

> adb devices

> adb kill-server

open terminal from the folder where adb is located.

> Install [App Inspector](https://play.google.com/store/apps/details?id=bg.projectoria.appinspector&hl=en_US&gl=US) from the Play store

