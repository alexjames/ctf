# Natas

### Level 0

View page source in browser.

Password: *gtVrDuiDfck831PqWsLEZy5gyDz1clto*

### Level 1

Right click is disabled. Use `Chrome Developer Tools` -> `Sources to view source`.

Password: *ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi*

### Level 2

This is a bit more tricky. The body only links to an image. The image has nothing of interest. But it is stored at the path `files/pixel.png`. The directory `files` allows directory traversal, where there is a `users.txt`.

Password: *sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14*

### Level 3

There's a hint saying that not even Google can find this page. This hinted at there being a `robots.txt` file that stops browsers from indexing pages. There is a `Disallow` section for a path named `s3cr3t`. Browsing that path reveals another `users.txt` file.

Password: *Z9tkRkWmpt9Qr7XrR5jWRkgOU901swEZ*

### Level 4

You are greeted with the message `You are visiting from "http://natas4.natas.labs.overthewire.org/index.php" while authorized users should come only from "http://natas5.natas.labs.overthewire.org/"`. There is a refresh button. Clicking on it sends another request with the HTTP header - 
```
Referer: http://natas4.natas.labs.overthewire.org/index.php
```
Use Burp suite to intercept and modify this request to the one from the message.

Password: *iX6IOfmpN7AYOQGPwtn3fXpbaJVJcHfq*

### Level 5
Look for the cookie `loggedin=0`. Change it to `loggedin=1`.

Password: *aGoY4q2Dc6MgDq4oL4YtoKtyAg9PeHa1*

### Level 6
Source code references a file that contains the secret. Input the secret and get to the next level.

Password: *7z3hEENjQtflzgnT29q7wAvMNfZdh0i9*

### Level 7
There is a hint saying the password is stored in `/etc/natas_webpass/natas8`. The url has a `page` parameter, hinting we should try getting to this path. We navigate to `http://natas7.natas.labs.overthewire.org/index.php?page=/etc/natas_webpass/natas8` to get the answer.

Password: *DBfUBfqQG69KvJvJ1iAbMoIpwSNQ9bWe*
