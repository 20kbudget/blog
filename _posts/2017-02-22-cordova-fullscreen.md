---
layout: post
title: Fullscreen on Cordova
---

To launch and app fullscreen and force landscape mode, this are 
the two preferences that needs to be added in the config.xml file:

```
<preference name="Fullscreen" value="true" />
<preference name="Orientation" value="landscape" />
```

A complete list of preferences can be found on [the docs][configxml].

[configxml]: https://cordova.apache.org/docs/en/latest/config_ref/
