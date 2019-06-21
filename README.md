# smile
Linux Face Unlock

## Existing Tools
Possibilities:
- [deepakgouda/faceunlock (Ubuntu)](https://github.com/deepakgouda/faceunlock) - Python, based on face_recognition library. Hooks directly into Ubuntu dbus.

- [devinaconley/pam-facial-auth](https://github.com/devinaconley/pam-facial-auth) - Slightly outdated opencv calls. Appears to use grayscale images. Forked [here](https://github.com/ARandomOWL/pam-facial-auth).

Ruled out:
- [AUR pam-face-authentication](https://aur.archlinux.org/packages/pam-face-authentication/) - Relies on outdated qt4/opencv. Last update upstream: 2013.

## Methods
Options:
1. Hook or patch the lock screen application.
2. Add PAM module.

#2 is the preferred option but depends on the lock screen application supporting PAM.

Lock screen applications known to support PAM:
- i3lock

PAM Resources:
- ￼https://github.com/beatgammit/simple-pam - PAM module example.
