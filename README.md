# Consensys-SVR4
Restoring a lesser-known Unix System V Release 4/i386 distribution from the early 90s.

## The Goal ##
To collect/recover and share a complete, runnable distribution of the Consensys SVR4 Unix system for Intel 386 (and later) PCs. Gather experience, collect docs.

## The Starting Point ##
Three boot disks - 5-1/4 inch 1.2M floppies containing the first level installation. Check the images directory for details.

## Intro ##
In the early 90s, after Sun Microsystems and AT&T (Unix System Laboratories) merged BSD Unix and Unix System V into Unix SVR4, a plethora of implementations for the Intel 386 platform arrived. From AT&T itself, from Sun (Solaris), from Novell (Unixware) and a number of others. One of them was Consensys Corp. of Dallas, TX.

Time has erased the reasons I chose the Consensys variant over one of the others, it may have been price. Anyway, the package arrived, containing 3 floppies, a 3M tape cartridge and manuals. Being busy at the time, I never got around to install the system. The tape and the manuals got lost (or ditched) in one of many moves, but the floppies survived.

Along with a lot of other computer-related stuff, some of it dating back to the late 70s, the floppies popped up during a cleaning process in 2017. The intention was to get rid of all or most of it, but curiosity won and a lot of stuff survived, including the Consensys floppies.

I attempted to boot them, succeeded to some degree and have been on the outlook for the rest of the system since. Not succeeding - and as we enter 2023 with absolutely nothing about Consensys on the net except some press releases, this repository is a final attempt. If you have anything that may point in the right direction, please let me know.

What we have here is a good start. The 3 floppies contain an amazing number of files, and looking at the content is an apt reminder of the complexity (and sheer volume of files) that made up the SVR4 system. With some trickery the 3 floppies can deliver a running system with a shell prompt, but it's not useful beyond proving that it runs.

![Consensys-diskettes](https://user-images.githubusercontent.com/3629880/211197261-0c3f907a-3a04-4f0c-9943-84782dd43199.jpeg)

Consensys Inc. released several updates (enhancements, bug fixes) to the system after the initial release in 1992, but got a reputation for bad customer support and sales didn't take off. They turned their attention to the fast growing Windows NT market and created a Unix SVR4 product called Portage which allegedly was "a complete integration of UNIX SVR4 with Windows NT". The product sold for $500 in 1995, but again the market was crowded (CygWin, NutCracker and more) and Consensys didn't last for long.
## Phase II ##
Three boot diskettes don't get us very far. Boot a bare bones system and play around a little, nothing more. The distribution from which the diskettes came, included a (long gone) tape cartridge containing the rest of the system. IOW - it was assumed that the target systems had a cartridge drive and a SCSI subsystem. So, even if I still had the cartridge, it would have been of little practical value.

What I didn'n know until recently (december 2024) is that there was also a floppy-only distribution of the system, 60+ 3.5" diskettes. Not only that, the person who shared this information had kept backup copies of the entire distribution and volunteered to share the images, now available in the `images` directory.  In the near future, I plan to create, configure and share a running VirtualBox disk image, possibly images for other emulators too (like QEMU which is the one I'm using the most).
![StorageOpen](https://github.com/user-attachments/assets/6268e763-949c-44a2-9bfb-3ffc6872a271)
