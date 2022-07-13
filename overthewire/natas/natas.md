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
