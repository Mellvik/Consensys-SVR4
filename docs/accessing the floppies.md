== Accessing the floppies ==

Unsurprisingly, the 3 boot floppies contain System V file systems which means the content is readable via other systems, such as Linux. Ubuntu Desktop 22 is a good choice.

Floppy 1 boots a Unix kernel and starts the installation process. The initial boot program occupies the first 15k bytes of the floppy, deferring the start of the file system to block 30. To mount this volume, use the following Linux command: `mount -o loop,offset=15360 ./Consensys-unix-1.img ./mnt` or whatever names fit your setting. Obviously the mount point must be created first, using the `mkdir` command.

The next two floppies can be mounted directly, no offset: `mount -o loop ./Consensys-unix-2.img ./mnt` etc. 
