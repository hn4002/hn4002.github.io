# Tips

index.html - works normally. Displays the content when we go to the site.


rest.json - github returns it like a normal json file with "application/json" content-type.

```
 $ curl -kv https://hn4002.github.io/rest.json
*   Trying 185.199.109.153...
* TCP_NODELAY set
* Connected to hn4002.github.io (185.199.109.153) port 443 (#0)
* ALPN, offering h2
* ALPN, offering http/1.1
* Cipher selection: ALL:!EXPORT:!EXPORT40:!EXPORT56:!aNULL:!LOW:!RC4:@STRENGTH
* successfully set certificate verify locations:
*   CAfile: /etc/ssl/cert.pem
  CApath: none
* TLSv1.2 (OUT), TLS handshake, Client hello (1):
* TLSv1.2 (IN), TLS handshake, Server hello (2):
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (IN), TLS handshake, Server key exchange (12):
* TLSv1.2 (IN), TLS handshake, Server finished (14):
* TLSv1.2 (OUT), TLS handshake, Client key exchange (16):
* TLSv1.2 (OUT), TLS change cipher, Client hello (1):
* TLSv1.2 (OUT), TLS handshake, Finished (20):
* TLSv1.2 (IN), TLS change cipher, Client hello (1):
* TLSv1.2 (IN), TLS handshake, Finished (20):
* SSL connection using TLSv1.2 / ECDHE-RSA-AES256-GCM-SHA384
* ALPN, server did not agree to a protocol
* Server certificate:
*  subject: C=US; ST=California; L=San Francisco; O=GitHub, Inc.; CN=www.github.com
*  start date: May  6 00:00:00 2020 GMT
*  expire date: Apr 14 12:00:00 2022 GMT
*  issuer: C=US; O=Cloud Services; OU=Operations; CN=SSL-SG1-GUSSC
*  SSL certificate verify ok.
> GET /rest.json HTTP/1.1
> Host: hn4002.github.io
> User-Agent: curl/7.54.0
> Accept: */*
>
< HTTP/1.1 200 OK
< Content-Length: 63
< Server: GitHub.com
< Content-Type: application/json; charset=utf-8
< Strict-Transport-Security: max-age=31557600
< Last-Modified: Wed, 15 Mar 2017 23:01:14 GMT
< ETag: "58c9c7ba-3f"
< Access-Control-Allow-Origin: *
< Expires: Fri, 15 May 2020 18:31:59 GMT
< Cache-Control: max-age=600
< X-Proxy-Cache: MISS
< X-GitHub-Request-Id: E660:3488:27B95:2D83F:5EBEDDC2
< Accept-Ranges: bytes
< Date: Fri, 15 May 2020 18:21:59 GMT
< Via: 1.1 varnish
< Age: 0
< X-Served-By: cache-bur17520-BUR
< X-Cache: MISS
< X-Cache-Hits: 0
< X-Timer: S1589566920.501890,VS0,VE32
< Vary: Accept-Encoding
< X-Fastly-Request-ID: d40ca71948c292afa49f6b205a269a3db83f390b
< Connection: Keep-Alive
<
{
    "status": "OK",
    "message": "This is working!!!!!!"
}
* Connection #0 to host hn4002.github.io left intact

```

# For Testing

Use following URL:

    * https://hn4002-github.localhost.net/



