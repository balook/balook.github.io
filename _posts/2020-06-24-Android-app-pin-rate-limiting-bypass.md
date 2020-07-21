---
layout: default
---

# Android pin rate limiting bypass

The bug is in private program .

There is a feature to lock mobile app with pin . But only 3 attempts. If we attempt wrong pin. The app logouts.
But there is a misconfig in this feature. If you enter the pin 2 times. close the app and open the app again you will get another 3 attempts . So the rate limiting bypassed by closing and calling the main activity
You can launch the main activity as many times as you want with adb

```
while true;do adb shell am start -a android.intent.action.VIEW -n com.redacted/com.redacted.MainActivity;sleep 4;done
```

while the sleep time you can enter the pin 2 times and again the main activity will be called so you can enter pin again.


## Impact : 

Android app auth pin's rate limiting bypassed

[back](./)
