---
layout: post
title: "Disable Android File Transfer autolaunch"
date: 2014-09-05 14:15:50
categories: android
---


If you are an Android user, you probably know the pretty useful **Android File Transfer app**. It allows you to handle files on your device as you would proceed with an USB key.

![Android File Transfer screenshot]({{ site.url }}/assets/posts/android_file_transfer/android_file_transfer.png)

But this application is obsessive about launching automatically each time you plug your device in your computer. If, as I am, you sometimes plug it in just for charge or development purposes, you don’t want Android File Transfer to auto launch.

And, Oh miracle ! Here is the solution to disable that behavior :
<br /><br />

  1. Close **Android File Transfer** app
  2. Run **Activity Monitor** and kill the Android File Transfer process
  3. Go to where you installed the app (probably in the /Applications folder)
  4. Right click on the package and Show package contents
  5. Go in the **./Contents/Resources** folder
  6. Rename Android File Transfer Agent in **Android File Transfer Agent_STOPTHATNOW**
  7. Do the same for the **/Users/yourusername/Library/Application Support/Google/Android File Transfer** file

<br />
Et voilà ! The app won’t auto launch anymore and you can now peacefully plug in your device !

![Happy meme]({{ site.url }}/assets/posts/android_file_transfer/happy_meme.gif)
