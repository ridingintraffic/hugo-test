---
layout: single
title: qmk
description: qmk notes
---

# qmk 
there is a bunch of qmk stuff out there
this is what you need for qmk and the ergodox ez keyboard… 

[https://docs.qmk.fm/](https://docs.qmk.fm/ "https://docs.qmk.fm/") - qmk documentation 

[https://www.pjrc.com/teensy/loader_linux.html
](https://www.pjrc.com/teensy/loader_linux.html
 "https://www.pjrc.com/teensy/loader_linux.html")


***if you are programming it with the qmk toolbox make sure that your have karabiner elements turned off


## docker images
qmk builder can be done via docker.  This means that it is way easier to build than dealing with all the dependencies for building, just use docker.
 ```
 docker run -e keymap=default_modded -e keyboard=ergodox_ez --rm -v $('pwd'):/qmk:rw edasque/qmk_firmware
 docker run -e keymap=ridingintraffic -e keyboard=ergodox_ez --rm -v $('pwd'):/qmk:rw edasque/qmk_firmware
 docker run -e keymap=ridingintraffic -e keyboard=planck/rev4 --rm -v $('pwd'):/qmk:rw edasque/qmk_firmware
```

location for qmk build and install
[https://github.com/qmk/qmk_toolbox/releases](https://github.com/qmk/qmk_toolbox/releases "https://github.com/qmk/qmk_toolbox/releases")

