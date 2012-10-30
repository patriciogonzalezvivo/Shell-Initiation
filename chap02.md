# 2. FileSystem & Directory Structure 

# Directory Structure

`/`		This is the root directory which should contain only the directories needed at the top level of the file structure.

`/bin`	This is where the executable files are located. They are available to all user.

`/dev`	These are device drivers.

`/etc`	Supervisor directory commands, configuration files, disk configuration files, valid user lists, groups, ethernet, hosts, where to send critical messages.

`/lib`	Contains shared library files and sometimes other kernel-related files.

`/boot`	Contains files for booting the system.

`/home`	Contains the home directory for users and other accounts. (`Users` on MacOS)

`/mnt`	Used to mount other temporary file systems, such as cdrom and floppy for the CD-ROM drive and floppy diskette drive, respectively (`/Volumes` on MacOS)

`/proc`	Contains all processes marked as a file by process number or other information that is dynamic to the system. 

`/tmp`	Holds temporary files used between system boots

`/var`	Typically contains variable-length files such as log and print files and any other type of file that may contain a variable amount of data

`/sbin`	Contains binary (executable) files, usually for system administration. For example fdisk and ifconfig utlities.

`/usr`	Used for miscellaneous purposes, or can be used by many users. Includes administrative commands, shared files, library files, and others. You can see how the structure repeats it self inside this folder. 

`/usr/bin`	

`/usr/etc`

`/usr/include`

`/usr/lib`

`/usr/local`

`/usr/share`

`/usr/sbin`

## User / Group / Others

There are three types of accounts on a Unix system:

Root account: This is also called superuser and would have complete and unfettered control of the system. A superuser can run any commands without any restriction. This user should be assumed as a system administrator.

System accounts: System accounts are those needed for the operation of system-specific components for example mail accounts and the sshd accounts. These accounts are usually needed for some specific function on your system, and any modifications to them could adversely affect the system.

User accounts: User accounts provide interactive access to the system for users and groups of users. General users are typically assigned to these accounts and usually have limited access to critical system files and directories.

Unix supports a concept of Group Account which logically groups a number of accounts. Every account would be a part of any group account. Unix groups plays important role in handling file permissions and process management.

Managing Users and Groups:
There are three main user administration files:

`/etc/passwd` Keeps user account and password information. This file holds the majority of information about accounts on the Unix system.

`/etc/shadow` Holds the encrypted password of the corresponding account. Not all the system support this file.

`/etc/group` This file contains the group information for each account.

`/etc/gshadow` This file contains secure group account information.