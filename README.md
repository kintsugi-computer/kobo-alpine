# Kobo-Alpine

A small repository of APK packages created to support running
Alpine Linux with X11 in a chroot on a Kobo eReader.

## Contents

* [kobo-fbink](https://github.com/kintsugi-computer/kobo-fbink): NiLuJe's FBInk utility and library compiled for Alpine Linux
* [kobo-fbink-xdamage](https://github.com/kintsugi-computer/kobo-fbink-xdamage): Shuhumi's FBInk-XDamage utility compiled for Alpine Linux
* [x11-touch-mouse](https://github.com/kintsugi-computer/x11-touch-mouse): Translate touchscreen events into X11 mouse events

## Quick Start

As root, add the URL of the repository to /etc/apk/repositories:

```
echo "https://kintsugi-computer.github.io/kobo-alpine/v3.22/kintsugi" >> /etc/apk/repositories
```

Copy the public key file to /etc/apk/keys:

```
cd /etc/apk/keys
wget https://kintsugi-computer.github.io/kobo-alpine/kintsugi.computer@protonmail.com-6
9ee4df3.rsa.pub
```

Update the local package database and install the packages:

```
apk update
apk add kobo-fbink-xdamage x11-touch-mouse
```
