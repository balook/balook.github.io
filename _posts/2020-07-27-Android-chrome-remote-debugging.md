---
layout: default
---


# Android chrome remote debugging


1. Install chrome on Android
2. connect to the android from pc through adb

you can connect throuh wireless or wired way (usb cabl3)

Install [adb root apk](https://play.google.com/store/apps/details?id=com.ttxapps.wifiadb&hl=en) to connect in a wireless way `(requires root)`
```
adb connect 192.168.0.100
```

From pc navigate to chrome://inspect 
From Android browse any site in chrome

Now you can see those sites in chrome://inspect tab
inspect it and now you can see the mobiel screen of chrome in pc chrome

# Inspect tab
![](./assets/chrome.PNG)

# Remote Android tab

`Change the url in this tab. and load arbitrary url in webview of the app`

![](./assets/chrome2.PNG)


# how it helps you in Android bugbounty

1 Not only the sites you browse in chrome apk but also you can see the sites in android  webview

2 you can know the cookies of the sites loaded in android webview too. becaues you can view that in pc chrome. 

3 you can run commands like alert(1); and know whether it is loading javascript;

4 you can navigate to other sites in apk webview. what you want from pc chrome debugging.


If you want to know much more explore it on your own ;- 
Poke around with it

No thanks for reading the report :-

[back](./)
