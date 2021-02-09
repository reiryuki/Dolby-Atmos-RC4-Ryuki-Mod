# Dolby Atmos RC4 Ryuki Mod Magisk Module

## Descriptions
- An EQ based on Dolby Atmos RC4 from @guitardedhero.
- Blobs from ZTE A2019 Pro for 64 bit, Lenovo TB-7305I for 32 bit, & apk's from Razer Phone.
- Doesn't work with Read-Only build ROM and no space free left of system & vendor except dolby dms HIDL 1.0 is already present in ROM manifest.xml.

## Requirements
- Android 9, 10, or 11
- Magisk installed

## Installation Guide
- Remove another Dolby module with different name
- Reboot
- Install via Magisk Manager or Recovery
- Reboot (reboot twice don't reflash, if you have Magisk sepolicy.rule bug)

## Optional
- If using multiple audio mods, use one of these bellow, don't use both!:
  - AML Module v4.0  (recommended), or
  - ACDB Module (Android 10 and bellow only) (not recommended since now using media codecs patch).
- You can rename any other dap-default to dap-default.xml to use more bass enhancer boost. See /data/adb/modules_update/DolbyAtmos/system/vendor/etc/dolby/. Rename another .xml to .mod. Delete /data/vendor/dolby/dap_sqlite3.db if there before reboot.
- You can disable your in-built Dirac audio FX if you sure it's conflicting with Dolby. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.disable.dirac` `1`

  After that, reflash the module.

- You can disable your in-built MI Sound FX if you sure it's conflicting with Dolby. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.disable.misoundfx` `1`

  After that, reflash the module.

## Troubleshootings
- If Dolby effect is not triggered, then you need to enable Dolby data clean-up. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.cleanup` `1`

  After that, reflash the module.

- If you using Xposed, Riru EdXposed, or Taichi Magisk Module, exclude Dolby apps from their list to prevent SE policy patch denials.
- If installation failed with "I/O error", then you need to disable DM-Verity of your ROM first.
- If installation failed with error "Read-only file system" or "No space left on device", that is mean you using dynamic partitions.
- For dynamic partitions, you should use ROM which is RW build and at least 1 MB free left of system or vendor, such as LineageOS. Or just ask to your ROM builder to add dolby HIDL 1.0 to ROM manifest.xml.
- If SE policy patch doesn't work for your device, send logcats to dev, then try using force permissive method.
  Run at Terminal Emulator before flash:

  - `su`

  - `setprop dolby.force.permissive 1`

  After that, reflash the module.

- You can also use both permissive mode and SE policy rule if necessary:

  - `su`

  - `setprop dolby.force.permissive 2`

  After that, reflash the module.

- If Dolby force close, reboot twice (don't reflash). It's probably Magisk sepolicy.rule bug.
- Make sure manifest.xml is patched correctly.
- If anything goes wrong, see your logcats
  - "CANNOT LINK EXECUTABLE" mean your audio hw library is not supported

## Report Guide
- Send me full logcats using this app https://play.google.com/store/apps/details?id=com.dp.logcatapp
- Send all "audio_effects" files in system/etc and vendor/etc
- If you don't do above, it will be closed immediately

## Credits
- @guitardedhero
- @Foxtrot47
- @aip_x
- @aquahol
- @BanCodrut
- All people that helped and supports

## Telegram
- https://t.me/audioryukimods
- https://t.me/modsandco

## Donate
- https://www.paypal.me/reiryuki


           - Enjoy the Atmos 🎧 -
