# smile
Linux Face Unlock

## Existing Tools
[deepakgouda/faceunlock (Ubuntu)](https://github.com/deepakgouda/faceunlock)

[devinaconley/pam-facial-auth](https://github.com/devinaconley/pam-facial-auth)

[AUR pam-face-authentication](https://aur.archlinux.org/packages/pam-face-authentication/) - Relies on outdated qt4/opencv. Last update upstream: 2013.

## Methods
Options:
1. Hook or patch the lock screen application.
2. Add PAM module.

#2 is the preferred option but depends on the lock screen application supporting PAM.

Lock screen applications known to support PAM:
- i3lock

PAM Resources:
- ￼https://github.com/beatgammit/simple-pam - PAM module example.
