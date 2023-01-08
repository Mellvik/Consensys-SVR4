The Consensys SVR4 floppies are not immediately accepted by all emulators because they don't recognize the boot code on the first floppy. However, `QEMU` is - as usual - you friend. The `-no-fd-bootchk` option disables the check and attempts to boot regardless, which works.

Start off by creating a hard disk to be the installation target: `qemu-img create -f raw q120m.img 120M`
Consensys SVR4 requires at least 60M, so anything 120M and up is fine.

Then the installation can start using the command 
`qemu-system-i386 -k no -no-fd-bootchk -boot order=ac -machine isapc -hda q120m.img -fda Consensys-unix-1.img`
... or if you'd like to play around after the 3 floppies have been installed, use the `Consensys-unix-1-mod.img` image instead.
