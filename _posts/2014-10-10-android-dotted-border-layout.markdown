---
layout: post
title: "Android layout with dotted border"
date: 2014-10-16 15:32:50
categories: android
---

There’s no “native” way to give a layout a dotted border on Android.

To do that, you have to create a drawable representing your border and attach it to your layout.

Create a resource file in your drawable folder just as follow :

<script src="https://gist.github.com/Onra/a18ef07ce9464bd1377b.js"></script>

<br/>

The key properties for the dotted line here are _**dashWidth**_ and _**dashGap**_.
As said by their name, _**dashWidth**_ allows you to set the width of each dot and _**dashGap**_ the width of each gap between dots.

You could also specify some padding and corner radius properties to not make design lovers cry too much. ʘ‿ʘ

Then, just link this drawable to the background property of your layout.

<script src="https://gist.github.com/Onra/9b874afe34f2b2435336.js"></script>

<br/>
Run your app and... Tadaaa !

![Android Dotted Border screenshot](/assets/posts/android_dotted_border/android_dotted_border.png)

Get the complete source code <a href="https://github.com/Onra/android-experiments-dotted-border" target="_blank">here.</a>
