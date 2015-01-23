# 4d-plugin-curl
This is a 4D plugin implementation of [libcurl and cURL](http://curl.haxx.se).

Important
---
This plugin project is a subset from what was published as "OAuth".

Existing cURL@ commands have the same name and functionality, but their tokens (internal IDs) have changed.

To migrate existing methods, do the following:

1. Comment the code that calls cURL@ plugin commands.
2. Close 4DB.
3. Replace the plugin.
4. Uncomment the code.
 
New
---
**cURL Get executable**

Returns the path to the curl executable embedded in the plugin. You can use this with LAUNCH EXTERNAL PROCESS.

Version
---
* v14 is for v14 and above, Windows, OS X 10.8+. 32/64 bits.
* v11 is for v11 and above, Windows, OS X 10.6+. 32/64 bits. (Intel only)

Dependencies
---

The libary version has been updated.

**Mac OS X**

* libcurl/7.39.0
* OpenSSL/1.0.1j 
* zlib/1.2.8 
* libidn/1.29 
* libssh2/1.4.3
 
**Windows**

* libcurl/7.39.0
* OpenSSL/1.0.1j
* zlib/1.2.8
* libidn/1.29
* libssh2/1.4.3

|Protocol|Mac OS X|Windows|
|:-------:|:-:|:-----:|
|dict|◯|◯|
|file|◯|◯|
|ftp|◯|◯|
|ftps|◯|◯|
|gopher|◯|◯|
|http|◯|◯|
|https|◯|◯|
|imap|◯|◯|
|imaps|◯|◯|
|ldap|◯|◯|
|ldaps|◯|◯|
|pop3|◯|◯|
|pop3s|◯|◯|
|rtsp|◯|◯|
|scp|◯|◯|
|sftp|◯|◯|
|smtp|◯|◯|
|smtps|◯|◯|
|telnet|◯|◯|
|tftp|◯|◯|

|Feature|Mac OS X|Windows|
|:-----:|:-:|:-----:|
|IDN|◯|◯|
|IPv6|◯||
|Largefile|◯|◯|
|NTLM|◯|◯|
|SSL|◯|◯|
|libz|◯|◯|
