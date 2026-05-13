# Kobo-Alpine

A small repostory of APK packages created to support in running
Alpine Linux with X11 in a chroot on a Kobo eReader.

## Contents

* kobo-fbink: NiLuJe's FBInk utility and library compiled for Alpine Linux
* kobo-fbink-xdamage: NiMa's FBInk-XDamage utility compiled for Alpine Linux
* x11-touch-mouse: Translate touchscreen events into X11 mouse events

## Quick Start

Add the URL of the repository to /etc/akp/repositories.

Copy the public key file to /etc/apk/keys

Update the local package database by running `doas apk update`.
