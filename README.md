```
                    ___ __             __                    __   
.-----.-----.-----.'  _|  .---.-.-----|  |--.----.---.-.----|  |_ 
|     |  -__|  _  |   _|  |  _  |__ --|     |  __|  _  |   _|   _|
|__|__|_____|_____|__| |__|___._|_____|__|__|____|___._|__| |____|
```

# neoflashcart - the "flashcart firmware" for portable handhelds

## scope

* do one thing - emulators - and do it well
* act like flashcart, not like a whole linux distribution crammed on
  little device
* start as fast as possible straight to the ROM selector
* single binary for kernel + rootfs loadable in ram, as small as possible
* emulators are static independent ELFs loadable for each game separately
* treat games like they actually are - ROM files, not "objects" in database
* the whole card should be FAT32 and keep as low non-game files as possible
* no support for features like cloud syncs, video playback, streaming, etc.

## supported devices

* **anbernic rg351v** as this is currently most gbc-like linux handheld
  available and author has it on his desk all the time

## possible supported devices

* **anbernic rg351p/mp and other OGA clones** as it won't take much to adapt
  them and the MP looks actually promising
* **raspberry pi cm4 devices** if there would be any GBC/GBA like handheld
  released with this quite capable soc
* **rk3399 handhelds** if they finally got one on the market
* **amd64 generic target** for testing and modularity support, also might
  come useful for small-sized htpc or arcade cabinet setup using old hw

## downloads

not yet, will provide CI automated builds when they become usable

## documentation

see above, but the docs are quite a priority for me before it gets released
expect in-system help and dev docs

## y u no use arkos/351elec/batocera/retroarena/retropie/etc?

as I mentioned above, these are trying to cram the whole "multimedia" experience
into the little boards they target, and I want to focus only on playing emulated
games and be as bulletproof as possible, like the flashcarts are

think about it as ez-flash / sd2snes / everdrive / supercard / r4ds but for these
funky chinese handhelds
