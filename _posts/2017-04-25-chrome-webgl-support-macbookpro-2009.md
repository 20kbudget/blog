---
title: WebGL support on Chrome
---

My work laptop is an old __MacBook Pro (17-inch, Mid 2009)__ 
with the __NVIDIA GeForce 9600M GT 512 MB__ video card.

Firefox and Safari are both able to run my [current game experiment][conveyor]
fine, but Chrome on that machine has GPU-acceleration disabled 
by default because of some blacklist of unsupported / buggy 
hardware and drivers :(

A simple way to check if your browser supports or have
enabled WebGL is to visit [this test page][webgltest].
If you see a spinning cube then you are good to go.

My Chrome didn't passed that simple test, so I went on investigating
why… I know that my video card supports open gl and web gl, so 
this should be just a matter of tweaking some configuration
flags.

The two main config pages to look for are: **chrome://gpu/**
and the **chrome://flags**

For me, the first fix was to **enable** the i**chrome://flags/#ignore-gpu-blacklist**
flag and restart the browser! \o/

Hooray!

[conveyor]: https://github.com/20kbudget/conveyor
[webgltest]: https://get.webgl.org/
[aboutgpu]: chrome://gpu/
[aboutflags]: chrome://flags/
[ignoreblacklist]: chrome://flags/#ignore-gpu-blacklist
