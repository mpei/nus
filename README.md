# nus
NUS (NeoUS Keyboard Layout)

**NUS Changes/ToDo (Crossed out equals done)**

  * Add Left Mod4, necessary since Mod4 enables arrow keys and numpad
  * ~~Do not allow Mod4+Mod4 toggle since this leads to problems~~
  * ~~Switch \ and / since LMod3+/ is used  more often and it would be more convenient to have them closer~~
  * Write Windows driver for NUS
  * Write driver for Linux console
  * \ (RMod3) becomes RMod4
  * RCTRL becomes RMod4
  * RALT becomes RMod3
  * Lock of Mod4 is only LShift+CapsLock+Tab
  * Take care / correct ssharp in top row
  * Add FN lock

**Installation (Linux, Ubuntu)**

* Append contents of file NUS to /usr/share/X11/xkb/symbols/us
> ```cat nus >> /usr/share/X11/xkb/symbols/us```

**How to use setxkbmap**

* Query settings:
> ```setxkbmap -query```

* Modify Settings
> ```setxkbmap LAYOUT VARIANT -model GEOMETRY -options OPTIONS```

* Switch to NUS:
> ``setxkbmap us nus -model pc105```
