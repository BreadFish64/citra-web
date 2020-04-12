+++
date = "2020-04-11T08:00:00-08:00"
title = "The Android Port is Here"
tags = [ "citra-release" ]
author = "BreadFish64"
# placeholders
banner = "announcing-android.png"
forum = 67781
+++

## You can finally play 3DS games on the go!

Hello there emulation afficianados! Today is Easter, and to celebrate, we're rolling away the stone on one of our most requested additions: Android Support!

<!--more-->

That's right. You can finally play 3DS games on the go! *

The Android port has been a long time in the making, and some of the challenges presented by the port were tough eggs to crack. So we'd like to thank all the developers who worked to make this possible.

The Easter [bunnei](https://github.com/bunnei) for
* Leading the project

The developers of the [Dolphin emulator](https://dolphin-emu.org) for
* The frontend that we heavily borrowed from
* The Aarch64 machine code emitter

[BreadFish64](https://github.com/BreadFish64) for
* OpenGL ES improvements
* Faster memory access for Aarch64 (thanks to [MerryMage](https://github.com/MerryMage) for the original x86 implementation)
* Motion control support

{{< figure type="youtube" id="iiH2JtFADV8" title="I'm using tilt controls!" >}}

[liushuyu](https://github.com/liushuyu) for
* OpenGL ES bug fixes

[SachinVin](https://github.com/SachinVin) for
* Originally repurposed the Dolphin UI
* Adding initial OpenGL ES support
* Implementing most of the Aarch64 [dynarmic](https://github.com/MerryMage/dynarmic) backend

[Tobi](https://github.com/FearlessTobi) for
* Porting changes to the Dolphin frontend since the original implementation
* Porting realtime audio from [yuzu](https://yuzu-emu.org)

[weihouya](https://github.com/weihuoya) for
* Implementing AAC decoding for Android
* Various performance improvements

[zhaowenlan](https://github.com/zhaowenlan1779) for
* The keyboard applet implementation

Many recent improvements to desktop Citra were also motivated by the Android release such as [Disk Shader Caching](https://github.com/citra-emu/citra/pull/4923), Proper [Texture Format Reinterpretation](https://github.com/citra-emu/citra/pull/5170), [Splitting Frame Presentation and Emulation into separate threads](https://github.com/citra-emu/citra/pull/4940) and more.

## So what can you expect from the Android port of Citra?

The app is still in beta. So while we've tried to squash the bugs we've come across, you may run into the occasional glitch. If you run into any major problems, please report them to us on our Discord server or forum, and we'll try to organize them.

{{< figure type="youtube" id="Is1IviWcX-Q" title="Uh, where are you going Mario?" >}}

The app requires a minimum of 64 bit Android Oreo, and OpenGL ES 3.2 support. These are relatively high requirements; however, they allow us to ensure that every device which can run Citra will have a reasonably good experience. We recommend a device with a Snapdragon 835 or better. Experiencing may vary greatly depending on the quality of your device's GPU drivers.

You can grab the app now on the [Google Play Store](https://play.google.com/store/apps/details?id=org.citra.citra_emu). The app is free, but we would appreciate it if you contributed to our ~~Cadburry Creme Egg~~ development and server upkeep funds by [becoming a Patron](https://www.patreon.com/citraemu) or unlocking dark mode for !!!insert price here!!!.

\* The Citra Emulator Project is not responsible for any bodily harm or injury that may result from leaving your home, including - but not limited to - sunburn, being hit by a runaway train, catching a highly contagious disease, or getting mauled by a polar bear.

Please do not use Citra while walking, driving, or otherwise locomoting.
