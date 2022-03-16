# Remove bloat from your Android

In our time, Android phone came with preinstalled apps that you can't remove directly on your smart phone. These apps can be really intrusive  and not very useful. 

So I'm going to show you how to remove these thanks to the help of ADB (Android debug Bridge) which is a tool made by Google for developers. 

## Installation on Windows

So first of all you need to install ADB on your PC , through this link [Android SDK](https://dl.google.com/android/repository/platform-tools-latest-windows.zip). 

Then extract the ZIP file. Open the folder that the extraction made, and open up a command prompt by holding Shift and Right Clicking within the folder then click the “Open command window here” option.

## Connection

Plug your smartphone to your computer but before that you need to activate <u>USB debugging</u> mode in your smartphone. This is a different process for all smartphone, so just do a quick google search to find how to do this. 

So after doing that, in the command prompt that you've open before type <u> adb devices</u> , and on your phone you should see a prompt to allow or deny USB debugging access, of course click "OK" or "Allow". And if the operation is successful you should see the name of your phone in the command prompt. 

> adb devices

## Utilization 

So to remove any app, you need to have the package name. To find that, I recommend downloading  [App Inspector](https://play.google.com/store/apps/details?id=bg.projectoria.appinspector&hl=en_US&gl=US) from the Play Store. Once you have the app launch it and press on an application. You're going to many information, but the only thing useful is the package name, it should look like that : . 

If you want to remove it, use this command in your command prompt :

>  pm uninstall --user 0 "package name"

And when you've uninstall every package, use this command to close the daemon server :

> adb kill-server

And that's it for this tutorial, hope this help to remove every bloatware from your phone. And if you don't know what to remove and what not just google "Bloatware on "brand your phone"". I might make txt file with everything you can remove. 



Sources : 

https://www.xda-developers.com/install-adb-windows-macos-linux/

