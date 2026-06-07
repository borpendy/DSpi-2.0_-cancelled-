Unfortunately i'm not developing this version further as I am not happy with the form factor, go see the dspi3 for the latest version thats much better.
I'll leave all the files up anyway but no new dev will be done.
# DSpi-2.0
The DS-pi 2.0 is the 2nd, and latest generation of the DS-pi project, a project with the goal of creating an open source dual screen gaming handheld, aimed at DS and 3DS emulation. Like the previous version, the DS-pi 2.0 is built off the Raspberry PI CM5, a small ARM based processor compute module, running a port of debian linux. Improvements over the original DSpi include a signifiantly better enclosure (resin printing option), and 720p main screen, allowing for use of steam-link and regular steam (mileage may vary, it's still a raspberry pi underneath). 

# Emulation capabilities
System performance is as expected from a standard raspberry pi 5. The system should be able to confortably emulate DS, PS1, PSP and any systems below that. I have also had good results with 3ds emulation, using the Borked3DS emulator, and some light PS2 and GC games may be playable. Regular steam also works, using the box86 and wine translation layers, however the number of playable games is limited. Streaming games should also be possible via steam-link or any other streaming methods.

# System Specifications

- Uses any Pi CM5 module (however the CM5 lite 8GB wifi is highly recommended) with 4 A76 cores at 2.4GHz.
- 1280x720 main display + 800x480 secondary display, with capacitive touch on both screens.
- Stereo speakers, using PCM5102 DAC + NS4150B amplifier, over the I2S interface.
- Headphone output, sharing the same PCM5102 DAC + PAM8908 Headphone AMP, speaker muting is enabled through the 3.5mm jack.
- 5000 Mah LiPo battery, with USB-PD charging enabled using the BQ24192 1S BMS, and HUSB238 PD controller..
- Full size controller using RP2040, and the GP2040CE firmware, using dual analog 3ds slide pads.
- Full 3d printable chassis, with both FDM and resin options available, using GBA SP hinges.

In addition to the changes in spec, this generation has also undergone a complete redesign of the internal electronics, to make use of the Modu-PI motherboard, more information here: https://github.com/borpendy/Modu-PI. This allows for a degree of seperation between the main motherboard, and controller daughterboard. If anyone wants to have a shot at improving the controller board (IMU, RGB ect), this should make things way easier for you.

## Other notes
Again this project is experimental, and not all things will work perfectly. This project has been an interesing journey, but unless you really want a linux handheld, I would suggest buying a current android handheld. If you are interested in how these devices are designed however, I encourage you check out the schematics above. Most of all, its cool that individual people can now make full products, and if you're thinking about doing someting similar, I highly recommend the experience.
