What's in the images:

- `Consensys-unix-[1-3].img` - the original floppy images, 1.2MB.
- `Consensys-unix-2-mod.img` - a minor modification to the 2nd floppy to eliminate the need for a license key.
- `Consensys-unix-1-mod.img` - Booting from this image will start an interactive shell just before the install procedure is about to ask for  the 'Foundation set' - see image below.

The shell provides the ability to poke around in the system, but the utilities are limited and the poking not all that useful.

<img width="742" alt="Skjermbilde 2023-01-06 kl  13 59 17" src="https://user-images.githubusercontent.com/3629880/211206110-a02c6eec-eb63-4036-ae0c-5724c7e1ebfa.png">

It seems reasonable to expect that the disk image created and partly filled at this point should be mountable - even bootable if we could find a kernel to boot from. However, I've not been able to get the Linux sysv filesystem implementation to recognize the image. Reason remains unknown.
