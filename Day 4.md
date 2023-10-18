## Further on Linux
#### Linux File Hierarchy
- Linux have a special file system which is a directory structure that the OS use.
- **System files** are files used by the the system software. As it is *Local disk C:* for **Windows** It's *root directory(/)* for **Linux**.
#### File structure in detail
1. **/ (root)**
	- Every single file and directory starts from the root directory
	- The only root user has the right to write under this directory
	- /root is the root user's home directory, which is not the same as **/**
2. **bin - Binary executables**
	- Essential command binaries that need to be available in single-user mode; for all users. Ex: *cat, ls, cp, pwd*
3. **/boot - Boot loader files**
	- Kernel initrd, vmlinux, grup files are located under /boot.
			Ex: *initrd.img-2.6.32-24-generic, vmlinuz-2.6.32-24-generic*
4. **/dev - Essential Device files**
	- These include terminal devices, USB, or any device attached to the system
			Ex: */dev/tty1, /dev/usbmon0*
5. **/etc et cetera**
	- Contains configuration files required by all programs. This also contains startup and shutdown shell scripts.
			Ex: */etc/resolv.conf, /etc/logrotate.conf.*
6. **/home - Home directory**
	- Home directories for all users to store their personal files.
			Ex: */home/remi*
7. **/lib - Libraries essential for the binaries in /bin & /sbin**
	- Library filenames are either Id or lib*.so.*
			Ex: *Id-2.11.1.so, libncurses.so.5.7*
8. **/media - Mount points for removable media such as CD-ROMS**
	- Temporary mount directory for removable devices.
			Ex: */media/cdrom* for CD-ROM, */media/floppy* for floppy drives, */media/cdtrcorder* for CD writer
9. **/mnt - Temporarily mounted file**
	- Temporary mount directory where sysadmins can mount filesystems.
10. **opt - Optional application software packages**
	- Contains add-on applications from individual vendors. Add-on applications should be installed under either /opt/ or /opt/ sub-directory
11. **/sbin - Essential system binaries**
	- Just like /bin, /sbin also contains executables. The Linux commands located under this directory are used by system administrator, for system maintenance purpose.
12. **/tmp - Temporary Files**
	- Directory that contains temporary files created by system and users.
	- Files under this directory are deleted when the system is rebooted.
13. **/usr - User Utilities**
	- Contains binaries, libraries, documentation, and source-code for second level programs
	- /usr/bin contains binary files for user programs. If you can't find a user binary under /bin, look under /usr/bin. For example: at, awk, cc. less, scp
	- /usr/sbin contains binary files for system administrators. If you can't find a system binary under /sbin, look under /usr/sbin. For example: *atd, cron, sshd, useradd, userdel*
	- /usr/lib contains libraries for /usr/bin and /usr/sbin.
	- /usr/src holds the Linux kernel sources, header-files and documentation.
#### Text Editors
- Programs that are used for text processing
- Linux command line text editors
	- **VIM**
	- **Nano**
	- **Emacs**
- Linux Graphical Text editors
	- **Sublime
	- **VS-code
	- **Gedit
##### VIM
- A very powerful, but at the same time it is cryptic
- Have two modes: Command and Insert
- To use Linux commands in vim : **":%!"
##### Nano
- The GNU nano text editor is a user-friendly, free and open-source text editor that usually comes pre-installed in modern Linux systems.
- Nano commands:
	- Ctrl + S - Save
	- Alt + U - Undo
	- Alt + E - Redo
	- Ctrl + X - Exit
	- Ctrl + Shift + C, X, V - Copy, Cut, Paste
	- Ctrl + R - appends text from other files
#### Linux User Management
- On computer system, person who uses the computer is called "user"
- Every Users have Group
- Users have their own file and application
- The users have privilege
- On Linux there's 2 kinds users.
	- Root id = 0
	- Normal User id starts with 1-999
- The root user have the power to do everything on Linux but if users want have a root access they add sudo infront of the command.
##### Creating Users
- On Linux, to create uses can use the following commands
	- Useradd -> simple
		- sudo useradd username
	- Adduser -> Detailed
		- sudo adduser usesrname
- The User files are stored inside /etc/passwd
- The User password are stored inside /etc/shadow
- When you create a user it creates a group with that name
- To access root user = > **sudo su**
----
