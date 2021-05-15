# Project-Serotonin

Project Serotonin is an effort to legally reverse engineer and patch the firmware on Fanatec steering wheel bases to remove anti-features/digital shackles and remove some limitations (under our own risk) that can be found in it.

Fanatec wheel bases disable force feedback when a non-official rim is connected, some may argue this is done in the name of safety, but it appears other manufacturers don't do this, so I decided to not buy this excuse.

While there exist hardware emulators for fanatec such as the ones made by Sim Racing Machines these are far from an ideal solution, for one they are costly compared to a simple QR mechanism without electrical connections + an external USB cable/wireless connection (such as those found in many third party rims), thus a software solution would be the best option.

This will also hopefully open the door to opening up the fanatec ecosystem and having more third party rim makers since Fanatec wouldn't hold a software monopoly over the bases anymore, thus other manufacturers could compete with their rim offerings, achieving a net positive for the community.

One may argue that why even use fanatec at all if they are so hostile to the community, this is true for those that can afford voting with their wallets, but this is not possible for less wealthy users such as myself, who while ended up with a fanatec wheel due to luck or a hand down (mine was obtained from a friend for example).

# Objectives

[x] Figure out how to decrypt the firmware files (this is currently done by dll injection into the firmware updater, a repository with the Rust code to do this will follow soon, but it would be nice to reimplement fanatec's own encryption mechanism which seems to just be using windows' cryptography and making such external tool extract the decryption key from the software).
[ ] Disassemble the firmware and figure out if it's even possible to patch out rim DRM from it or if it's a purely electrical solution.
[ ] Creating a user friendly tool to patch your own firmware with ease.

Currently I do development on a PS4 version of the CSL Elite, but it would be nice if after we figure out how to crack this one open patches for other wheels can also be made. I suspect most fanatec wheels (save for the DD ones maybe?) uses the same MCU, at least the old GT3 RS V1 and V2 seem to use the same microcontroller as the CSL Elite from some old forum posts I found.

# Wishlist

In the future it would be nice if we can add more features and overrides, such as:
[ ] The ability to patch DD bases to not need the podium QR for full torque (this one I can actually believe is done the way it's done because the hardware maybe can't take it).
[ ] The ability to patch non-PS4 CSL Elites to work with a PS4 (likely not possible if there is indeed a sony-specific lockout chip).

# Other things to do
[ ] Add images of the board and info on the MCU.
