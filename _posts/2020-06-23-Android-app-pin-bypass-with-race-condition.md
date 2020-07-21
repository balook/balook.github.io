---
layout: default
---

# Creative Android pin bypass with Race conditon

Hitting main activity multiple times app allowing to view any activity inside an app. without even entering the mobile pin.


## Bug 

Application has a mobile pin security. without entering the pin you cant enter into the app.


# Bypass 

But by calling internal activities like settings.activity and notifications.activity with race condition . The app is showing settings page ,profile page. but the problem is it only allow us to see for some seconds.So we need to automate it and take the screen shot by calling the activites .

```
for i in $(seq 20);do adb shell am start -a android.intent.action.VIEW -n com.redacted.android/.MainActivity -d "https://redacted.com/notifications";adb shell screencap /sdcard/tmp/$i.png;done

```

The above command run 20 times and take screen shot of frontend and save it in sdcard directory.


# Impact :

Attacker cant bypass the pin completely . but can view the content inside the app and know the sensitive info like . amount, profile info

[back](./)
