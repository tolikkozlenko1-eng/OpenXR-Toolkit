# OpenXR Toolkit — gaze DFR branch

This branch is the **buildable source** for [OpenComposite DFR](https://github.com/tolikkozlenko1-eng/opencomposite-dfr): one OpenXR API layer in the Primashock / OpenXR Toolkit slot. It is **not** OpenComposite itself.

Download the built layer: [opencomposite-dfr.zip](https://github.com/tolikkozlenko1-eng/opencomposite-dfr/releases/latest/download/opencomposite-dfr.zip).

What this branch adds on top of Matthieu Bucchianeri's Toolkit:

- One eye-tracked foveation circle for OpenComposite games. The circle works universally on those titles
- A game that draws each eye as its own picture gets the circle on that picture
- A game that draws both eyes into one wide side-by-side picture gets a circle in each half, when each half matches the per-eye aspect
- NVIDIA D3D11 variable rate shading (inner disk full rate, outside 1/16)

Build: Visual Studio 2022 (`v143`), `OpenXR-Toolkit.sln`, target `XR_APILAYER_MBUCCHIA_toolkit`, Release x64. The post-build copy/sign step can fail on paths with spaces. The DLL is still written to `bin\\x64\\Release`. Do not commit `nuget.exe`.

---

# OpenXR Toolkit

This software provides a collection of useful features to customize and improve existing OpenXR applications,
including render upscaling and sharpening, foveated rendering, hand tracking to controller input simulation,
image adjustments and other game-enhancing tweaks.

Please visit the official page at https://mbucchia.github.io/OpenXR-Toolkit/ for detailed instructions on how to download,
install, and use this software.

DISCLAIMER: This software is distributed as-is, without any warranties or conditions of any kind. Use at your own risks.

## Donate

Donations are welcome and totally optional. Please use [my GitHub sponsorship page](https://github.com/sponsors/mbucchia) to make one-time or recurring donations!

Thank you!

## Contributions

This software was created by Matthieu Bucchianeri and Jean-Luc Dupiot.

Logo and icons designed by RPthreenine.

User Experience designed by Andrew Lilley (FarFutureFox).

Additional contributions by James Lacey (Jabbah), Bernhard Berger, and Erik Uri.

Many thanks to the https://forums.flightsimulator.com/ community for the testing and feedback!
