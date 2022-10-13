

Original version pointed to revision 111
"three": "github:mozillareality/three.js#hubs-patches",

Hubs at this moment points to 141
MegaMotion pointined to "three": "^0.112.0",

All of these are super old with three being at r145

We'll try to update to 141 via hubs
was "three": "github:mozillareality/three.js#hubs-patches",
needs
https://github.com/MozillaReality/three.js/tree/hubs-patches-141

?2





#notes from discord
```
https://discord.com/channels/498741086295031808/535606666708910101/718933006315814943
Kevin Lee
 — 
06/06/2020
The features of bullet available in ammo are gated by what is exposed in ammo’s ammo.idl (which defines what classes and functions emscripten will “port”). Then, the features of ammo available in hubs are gated by three-ammo’s ammo-worker.js, as we run three-ammo (and thus ammo/bullet) in a worker thread. So three-ammo exposes a postmessage api to allow hubs proper to communicate with the physics system
```



# three-ammo

A [three.js](https://github.com/mrdoob/three.js/) wrapper for [Ammo.js](https://github.com/kripken/ammo.js/) that can run in a web-worker using Shared Array Buffers or PostMessage. Primarily for use with [Mozilla Hubs](https://github.com/mozilla/hubs).

[side by side comparison of running with/without a worker](https://twitter.com/i/status/1218263836303581184)

Also see:

[three-to-ammo](https://github.com/InfiniteLee/three-to-ammo)

[ammo-debug-drawer](https://github.com/InfiniteLee/ammo-debug-drawer)
