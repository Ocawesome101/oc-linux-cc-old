# oc-linux-cc
A Linux-like system for ComputerCraft's CraftOS.

This is my best attempt at creating a Linux-like shell written entirely in Lua. I have based it on ComputerCraft's CraftOS and
Lua scripting system.

I have copied many of the default CraftOS scripts, as they serve their purpose just fine. However, many of them have been renamed and otherwise edited slightly (to more greatly resemble Linux commands) by me.

I recommend installing this on a fresh Advanced Computer (Advanced Pocket Computers will be directly supported in a later update, and OC Linux should work on them now). However, it may work on standard Computers and Pocket Computers as well.

To install, simply run `pastebin run wMhFGDAr` on any computer.

Be warned, there are several caveats:
  - The system overwrites os.version() on startup, though this can be changed
  - This is by no means a perfect copy of Linux (there are limitations!)
  - This is STILL IN DEVELOPMENT.
  - For authenticity's sake, the default PATH is changed on every boot to completely REMOVE all /rom/* entries. This may break some programs.
  - I have tried to make sure that all of the default CraftOS APIs are still available, though I make no guarantees as to whether things will stay as they are.
  - As of release 0.5.0, /boot, /var, and /dev are unused. However, they will be in a future update!
  - As of release 0.5.0, there is no user account system implemented. This is something that is fairly high priority for me.
  - As of release 0.5.0, there is no package manager system in any way, shape, or form. However, I plan to add a package manager later.

 Some guidelines to follow while coding:
  - User-made APIs should be stored in and /usr/local/lib rather than /apis or wherever else.
  - Scripts are still to be written in Lua
  - User-made scripts should be stored in /usr/local/bin
  - Scripts should not modify any files in /bin, /usr/bin, /lib, /usr/lib, /dev, /boot, or /sbin, and should not delete any premade files in /etc. However, you may create files, and delete your own files (but ONLY YOUR OWN FILES) in /etc.
  
# Have fun!
