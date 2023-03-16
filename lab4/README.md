## UID: 905694345

(IMPORTANT: Only replace the above numbers with your true UID, do not modify spacing and newlines, otherwise your tarfile might not be created correctly)

# Hey! I'm Filing Here

This is the code to make a 1 MiB ext2 file with two directories, 1 regular file, and 1 symbolic link.

## Building

To build the program run 'make' in the lab4 directory.

## Running

To run the executable to create cs111 -base.img, run:
> ./ ext2 - create
To check that the file sysytem is correct, run:
> fsck.ext2 cs111-base.img
To create a directory to mnt your file system to, run:
> mkdir mnt 
To mount your filesystem, run
> sudo mount -o loop cs111 -base.img mnt

To test, run:
> python -m unittest
*You do not need to run 'make' because this will do it for you*

## Cleaning up

To unmount the filesystems, run:
> sudo umount mnt
To delete the directory, run:
> rmdir mnt

Run 'make clean' in the lab4 directory to clean up files. If you used the python test suite then it will run make clean for you, all you need to do is run 'rm -r __pychache__'.
