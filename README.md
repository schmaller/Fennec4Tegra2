# Fennec4Tegra2
 Build recent versions of Firefox for Android ("Fennec") for ARMv7/Cortex-A9 NON-NEON platforms (e.g. Tegra2) 

## Downloads
 You can find pre-compiled APKs in the [dist](https://github.com/schmaller/Fennec4Tegra2/tree/master/dist)
directory.

## History
This project is based on the patch from [Wryun](https://github.com/wryun/)
and his great work [firefox-ics-tegra2](https://github.com/wryun/firefox-ics-tegra2)
__Many thanks__
...to be completed...

## Patches
Besides the patches to build NEON-free binaries I focused on reducing
runtime overhead of needless "_features_" and __posh__ extenstions.
Due to the different handling of configure options in the android build
scripts this approach didn't seem to be too successful.  
I appreciate any hints for further performance improvements.

Furthermore the pre-compiled APKs use the following privacy (or accessibility) settings as default:
    pref("privacy.donottrackheader.enabled", true);
    pref("privacy.trackingprotection.enabled",true);
    pref("network.cookie.cookieBehavior", 1);
    pref("media.autoplay.enabled", false);
    pref("browser.ui.zoom.force-user-scalable", true);

## Devices
According to Wikipedia the following devices contain a Tegra2 SoC and may
now be provided with a modern web browser and decent surfing performance.  
I own a Samsung Galaxy Tab 10.1n and my impression is, that this build of Fennec
is slightly less stuttering than [Chromium 62 for Tegra2](https://forum.xda-developers.com/galaxy-tab-10-1/development/app-chromium-m56-optimized-tegra-2-t3550210),
 and of course faster than Firefox 52.
- ASUS Eee Pad Transformer
- Acer Iconia Tab A100
- Advent Vega
- Aigo n700
- Avionic Design Tamonten Processor Board
- CompuLab Trim-Slice nettop
- E-Noa Interpad
- Exper EasyPad
- Hannspree Hannspad
- Lenovo IdeaPad Tablet K1
- Lenovo ThinkPad Tablet
- MSI 10-inch (250 mm) tablet
- Malata Tablet Zpad
- Notion Ink Adam tablet
- Olivetti OliPad 100
- Point of View Mobii 10.1
- Samsung Galaxy Tab 10.1
- Toradex Colibri T20
- Toshiba AC100
- Toshiba Folio 100
- Velocity Micro Cruz Tablet L510
- ViewSonic G Tablet
- ViewSonic ViewPad 10s
- Zyrex Onepad SP1110
- Zyrex Onepad SP1113G