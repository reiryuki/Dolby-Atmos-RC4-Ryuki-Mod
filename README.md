# Dolby Atmos RC4 Ryuki Mod

## Descriptions
- An EQ based on Dolby Atmos RC4 from @guitardedhero.
- Bloobs known modded from ZTE A2019 Pro for 64 bit and Lenovo TB-7305I for 32 bit.
- Doesn't work with dynamic partitions

## Requirements
- Android 9, 10, or 11 64 and 32 bit devices
- Magisk installed
- Don't use with another Dolby module!

## Installation Guide
- Remove another Dolby module
- Reboot
- Install via Magisk Manager only
- Reboot

## Optional
- If using multiple audio mods, use one of these bellow, don't use both:
  - AML 4.0 supported
  - ACDB supported (Android 10 and bellow only for now)

## Troubleshooting
- If Dolby force close, just reinstall again.
- Make sure manifest.xml is patched correctly.
- Use Audio Compatibility Patch if you encounter processing problem.
- Bass enhancer boost headphone is modified in v1.5 and up. If you don't like it, just rename dax-default.orig to dax-default.xml.
- If se patch still fail even added to sepolicy.rule, then add `setenforce 0` to the top of service.sh.

## Attention!
- Reporting anything without sending full logcats and install process logs is ignored!
https://play.google.com/store/apps/details?id=com.dp.logcatapp

## Credits
- @guitardedhero
- dolby_dax.jar recompiled by @aip_x

           - Enjoy the Atmos 🎧 -
