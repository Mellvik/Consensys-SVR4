What's in the 1.2M images:

- `Consensys-unix-[1-3].img` - the original floppy images, 1.2MB.
- `Consensys-unix-2-mod.img` - a minor modification to the 2nd floppy to eliminate the need for a license key.
- `Consensys-unix-1-mod.img` - Booting from this image will start an interactive shell just before the install procedure is about to ask for  the 'Foundation set' - see image below.

The shell provides the ability to poke around in the system, but the utilities are limited and the poking not all that useful.

<img width="742" alt="Skjermbilde 2023-01-06 kl  13 59 17" src="https://user-images.githubusercontent.com/3629880/211206110-a02c6eec-eb63-4036-ae0c-5724c7e1ebfa.png">

It seems reasonable to expect that the disk image created and partly filled at this point should be mountable - even bootable if we could find a kernel to boot from. However, the Linux `sysv` file system implementation supports floppy disks only, so there seem to be no way to access this file system except from a 'real', running System V system. Which may be an interesting next step: Boot an old copy of Solaris 5/386, AT&T System V rel 4/386 or one of the other implementations available on the net.

Refer to this link https://kernel.org/doc/Documentation/filesystems/sysv-fs.txt for more details about the Linux `sysv-fs`.

## Complete-dist ##
This directory contains the floppy images of a complete Consensys SVR4.2 system. Also included is the serial and validation numbers, eliminating the need for the trickery which enabled the 1.2M boot diskettes to work.

<img width="742" alt="license numbers" src="./complete-dist/Consensys Unix SVR4.2 License.png">

