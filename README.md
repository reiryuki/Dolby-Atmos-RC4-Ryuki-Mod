# Dolby Atmos RC4 Ryuki Mod Magisk Module

## Descriptions
- An EQ based on Dolby Atmos RC4 from @guitardedhero.
- Blobs from ZTE A2019 Pro for 64 bit and Lenovo TB-7305I for 32 bit.
- Doesn't work with dynamic partitions (except dolby dms 1.0 is already present in ROM manifest.xml)

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
- You can rename any dap-default extension to .xml to use more bass enhancer boost. See /data/adb/modules_update/DolbyAtmos/system/vendor/etc/dolby/. Rename another .xml to .mod. Delete /data/vendor/dolby/dap_sqlite3.db if there before reboot.
- You can disable your in-built Dirac audio FX if you sure it's conflicting with Dolby. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.disable.dirac` `1`

  After that, flash/reflash the module.

- You can disable your in-built MI Sound FX if you sure it's conflicting with Dolby. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.disable.misoundfx` `1`

  After that, flash/reflash the module.

## Troubleshootings
- If Dolby effect is not triggered, then you need to enable Dolby data clean-up. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.cleanup` `1`

  After that, flash/reflash the module.

- If you using Riru EdXposed or Taichi Magisk Module, exclude Dolby apps from their list to prevent SE policy patch denials.
- If installation failed with "I/O error", then you need to disable DM-Verity of your ROM first.
- If installation failed with error "No space left on device", that is mean you using dynamic partitions.
- If SE policy patch doesn't work for your device, send logcats to dev, then try using force permissive method.
  Run at Terminal Emulator before flash:
  - `su`
  - `setprop dolby.force.permissive 1`
- If Dolby force close, just reinstall again.
- Make sure manifest.xml is patched correctly.
- Use Audio Compatibility Patch if you encounter processing problem. But usually don't need.
- If anything goes wrong, see your logcats
  - "CANNOT LINK EXECUTABLE" mean your hardware is not supported

## Attention!
- Reporting anything without sending full logcats and install process logs is ignored!
https://play.google.com/store/apps/details?id=com.dp.logcatapp
- Send run also:
  - `su`
  - `dumpsys media.audio_flinger`

## Credits
- @guitardedhero

## Telegram
- https://t.me/audioryukimods
- https://t.me/modsandco

## Donate
- https://www.paypal.me/reiryuki


           - Enjoy the Atmos 🎧 -
