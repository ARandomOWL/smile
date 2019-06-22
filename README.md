# smile
Linux Face Unlock

## Existing Tools
Possibilities:
1) [deepakgouda/faceunlock (Ubuntu)](https://github.com/deepakgouda/faceunlock) - Python, based on face_recognition library. Hooks directly into Ubuntu dbus. Requires python-face_recognition from AUR and python-opencv from pip. Can take up to 8 seconds to execute.

    - Limitations:
        * Easily spoofed with an image.
        * The facial recognition doesn't work if the face has any partial covering.

2) [devinaconley/pam-facial-auth](https://github.com/devinaconley/pam-facial-auth) - Slightly outdated opencv calls. Appears to use grayscale images. Forked [here](https://github.com/ARandomOWL/pam-facial-auth).


Ruled out:
3) [AUR pam-face-authentication](https://aur.archlinux.org/packages/pam-face-authentication/) - Relies on outdated qt4/opencv. Last update upstream: 2013.

## Methods
Options:
1. Hook or patch the lock screen application.
2. Add PAM module.

#2 is the preferred option but depends on the lock screen application supporting PAM.

Lock screen applications known to support PAM:
- i3lock

PAM Resources:
- ￼https://github.com/beatgammit/simple-pam - PAM module example.

## Other technology
- Apple's FaceID uses an infrared light to create an encoded depth map of the users face. 
  - This overcomes the limitations of spoofing the algorithm with an image.
