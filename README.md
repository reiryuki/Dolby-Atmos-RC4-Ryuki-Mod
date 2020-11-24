# Dolby Atmos RC4 Ryuki Mod Magisk Module

## Descriptions
- An EQ based on Dolby Atmos RC4 from @guitardedhero.
- Blobs known modded from ZTE A2019 Pro for 64 bit and Lenovo TB-7305I for 32 bit.
- Doesn't work with dynamic partitions

## Requirements
- Android 9, 10, or 11
- Magisk installed

## Installation Guide
- Remove another Dolby module
- Reboot
- Install via Magisk Manager only
- Reboot

## Optional
- If using multiple audio mods, use one of these bellow, don't use both:
  - AML 4.0 supported
  - ACDB supported (Android 10 and bellow only for now)
- You can rename dap-default extension to use more bass enhancer boost. See /data/adb/modules_update/DolbyAtmos/system/vendor/etc/dolby/

## Troubleshooting
- If SE policy patch doesn't work for your device, send logcats to dev, then try using force permissive method.
  Run at Terminal Emulator before flash:
  - `su`
  - `setprop dolby.force.permissive 1`
- If Dolby force close, just reinstall again.
- Make sure manifest.xml is patched correctly.
- Use Audio Compatibility Patch if you encounter processing problem.
- If you have some issues, like ringtones, alarm tones doesn't work, or calls opposite person doesn't hear, [do this fix.](https://t.me/audioryukimods/543)
- If this still doesn't work, use RC1 instead.

## Attention!
- Reporting anything without sending full logcats and install process logs is ignored!
https://play.google.com/store/apps/details?id=com.dp.logcatapp
- Send run also:
  - `su`
  - `dumpsys media.audio_flinger`

## Credits
- @guitardedhero

## Groups discussion
- https://t.me/joinchat/E-On6U9cxckhIlAnoPIYpw
- https://t.me/@modsandco

## Donate
- https://www.paypal.me/reiryuki


           - Enjoy the Atmos 🎧 -
