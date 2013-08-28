GuardianKernel-n7000
====================

Guardian Kernel is a android kernel with Mobiflage (https://github.com/x942/mobiflage) PDE (Plausable Deniable Encryption) built in. This version is for n7000 (Samsung Galaxy Note International)

How to use:

1) Use kernel with android that has the Mobiflage (https://github.com/x942/mobiflage) patches in place

2) using an adb shell enter "vdc cryptfs pde wipe [outer volume password]  [hidden volume password]"

3) All done. Please report any bugs :)


Notes: 

1) Use a strong password on both the outer and hidden volumes. For day-to-day use you should supply the decoy password.
This will activate standard mode, where the user can perform all their normal activities on the device, such as making calls
and browsing the web. All data saved to the device in standard mode will be encrypted but not hidden. It is favorable to use
PDE mode only when necessary and standard mode at all other times.

2) When wanting to use PDE mode reboot the device and enter the password for the hidden volume. this boots into PDE mode where
all of your files are hidden. You can ony view these files in this mode and they are hidden when the device is off or in standard mode
the user should save files in the deniable storage (PDE mode) and immediately reboot into standard mode when done. This 
limits the chances of hidden volume/files being discovered by an attacker.

3) Read the documentation here: users.encs.concordia.ca/~a_skil/mobiflage/ 

4) Many thanks to the authors of Mobiflage. :)


Linux kernel standard readme: https://github.com/yair/GuardianKernel-n7000/blob/master/README

