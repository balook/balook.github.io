---
layout: default
---

# Android Instagram ssl unpinning.

Download apk from this repo

[Instagram apk](https://github.com/itsMoji/Instagram_SSL_Pinning/blob/master/non-root/arm/Instagram_v148.0.0.33.121_227298996_minAPI19(armeabi-v7a)(nodpi).apk)

If your mobile is x86 architecture download x86 version of non root.

This apk got reverse engineered and u can intercept the traffic.
The repo above will be updated with new insta apk everytime when new instagram version release.

The problem with above apk is at the first time you install it . you can see the traffic but when u close the apk and try to log the traffic second time ... you get an error. To avoid it  clear the app data and cache data. and login again. now it works. and u can only the log the traffic if your burp version (2020.4 im using)is new and  having java 12 installed. 

Go to project settings > TLS > use custom protocols and ciphers  > select all tls protocols and ciphers too.

![](./insta.PNG)

# Now you can see the traffic

![](./insta2.PNG)

For bypassing ssl unpinning i used [xposed  module](./android-instagram-ssl-unpinning).

If you have any doubt dont contact me [@critical_b0y](https://twitter.com/critical_b0y)





[back](./)
