CVE-2019-5786 Chrome 72.0.3626.119 stable FileReader UaF exploit for Windows 7 x86. 

This exploit uses site-isolation to brute-force the vulnerability. iframe.html is the wrapper script that loads the exploit, contained in the other files, repeatedly into an iframe.

* host iframe.html on one site and exploit.html, exploit.js and wokrer.js on another. Change line 13 in iframe.html to the URL of exploit.html
* start chrome with the --no-sandbox argument
* navigate to iframe.html