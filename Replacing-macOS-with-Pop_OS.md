### To-Do before replacing macOS

1. Scroll down and read the cons of replacing macOS with any other OS. 
2. Download macOS, create a bootable installer for macOS. You will need this later to do firmware updates. [Instructions](https://support.apple.com/en-us/HT201372)

### Replacing macOS with [Pop!_OS](https://pop.system76.com/)

1. Download the .iso image from the Pop!_OS website. Download the **current** version, not the LTS version.
2. Make a bootable pendrive following these [instructions](https://support.system76.com/articles/live-disk/)
3. Shut down the mac, stick in the bootable drive. Power on and hold the option/alt key to reach the *EFI* option. Click on the *EFI boot* option
4. Choose a clean install if you want to replace macOS, partion and other stuff if you want to keeo macOS too. I did the former.

***

### Wifi drivers

First things first. [Instructions](https://askubuntu.com/a/60395)

***

### Camera

Follow the instructions on patjak's [FacetimeHD linux driver](https://github.com/patjak/bcwc_pcie/wiki)

***

### Software you may install from Pop!_Shop

1. Skype
2. VLC Media Player

***

### Cons

1. Firmware updates can only be done through macOS
2. No more three-finger drag, you do a tap-tap-drag
3. Significant dip in battery life not so significant if the OS you are replacing it with a 'light' one like pop_os

***

### Firmware Updates

Firmware updates can only be done through macOS. Go to the *recovery* mode of the Mac. Insert the USB drive with the bootable installer for macOS. Format the USB using Disk Utility, use the default options. Exit out of Disk Utility and then install onto it.

***

### References

1. [Switching from macOS to Pop!_OS](https://support.system76.com/articles/switch-from-macos-to-popos/)
