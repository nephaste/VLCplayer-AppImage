# VLCplayer-AppImage
![VLC](https://user-images.githubusercontent.com/581999/41001881-e33ecc94-691a-11e8-8974-5fcdfcb42f89.jpg)

Unofficial VLCplayer AppImage, VLC version (3.0.8) build from source.

## Why?
AppImage is a format for distributing portable software on Linux without needing superuser permissions to install the application  It tries also to allow Linux distribution-agnostic binary software deployment for application developers, also called Upstream packaging. Released first in 2004 under the name klik, it was continuously developed, then renamed in 2011 to PortableLinuxApps and later in 2013 to AppImage. [wikipedia](https://en.wikipedia.org/wiki/AppImage)

## Download
Download the AppImage from [here](https://github.com/cmatomic/VLCplayer-AppImage/releases/).

## How do I know it's safe?
As with most things you download from the Internet nowadays, you can't. But you can inspect the source code, improve it, decide for yourself whether to download the AppImage from the link above or create your own fork.

## Compatibility
This AppImage has been tested on the following GNU / Linux distros.
* #### Debian 10 buster
* #### OpenSUSE-Leap 15.1 KDE Live-x86_64
* #### Ubuntu xenial 16.04
* #### Ubuntu Bionic 18.04
* #### Ubuntu Disco 19.04
* #### Linuxmint 19.2 cinnamon-64bit
* #### Manjaro-xfce 18.1.0 stable-x86_64
* #### Mageia 7.1 Live-Plasma-x86_64
* #### MX-19


## Playing DVDs and Blu-rays
*  DVDs https://www.videolan.org/developers/libdvdcss.html

* Blu-rays

* vlc AACS ( install libaacs on your distro ) https://vlc-bluray.whoknowsmy.name/

*  alternative install makemkv https://www.makemkv.com/forum/viewtopic.php?f=3&t=7009


## Hardware video acceleration

* Arch wiki https://wiki.archlinux.org/index.php/Hardware_video_acceleration
* NVIDIA "vdpau" (mesa-vdpau-drivers;libvdpau)
* intel  "vaapi"(libva )
* AMD    "vaapi" and "vdpau"

## features not activated
* chromecast:"protobuf" bug in gnutls-bin, preventing it from working correctly (during the build the binary was segfaulting)on Ubuntu xenial https://trac.videolan.org/vlc/ticket/18329
* crystalhd: unusble without firmware (#934242)
* d3d11va: Windows only
* decklink: not in Debian/Ubuntu xenial
* directx: Windows only
* dxva2: Windows only
* fluidlite: fluidsynth is enabled
* freerdp: scheduled for removal (#888323)
* goom: not in Debian/Ubuntu xenial
* gst-decode: not needed when having libavcodec
* libtar: security issue (#737534)
* macosx : MacOX only
* mfx: currently not supported on Linux
* opencv: developer plugin not required by end users
* projectm: broken
* schroedinger: removed from Debian/Ubuntu xenial (#845037)
* sparkle: MacOS X only
* telx: incompatible with zvbi
* vpx: not needed when having libavcodec
* vsxu: not in Debian/Ubuntu xenial
* wasapi: Windows only

## Credits
This repo is mainly based on the work of [icflorescu](https://github.com/icflorescu/vlc-3-appimage), [Anupam Basak](https://github.com/anupam-git/vlc-appimage) and [darealshinji](https://github.com/darealshinji/vlc-AppImage).

## License

This repo is [ISC-Licensed](https://github.com/icflorescu/vlc-3-appimage/blob/master/LICENSE).
Please refer to [this page](https://www.videolan.org/legal.html) for VLC-related licensing stuff.
