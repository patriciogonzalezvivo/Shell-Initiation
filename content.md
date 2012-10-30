# About UNIX
http://www.bell-labs.com/history/unix/tutorial.html

# The Terminal 

Intro to bash. 
http://web.mit.edu/gnu/doc/html/features_toc.html
http://www.linuxtopia.org/online_books/advanced_bash_scripting_guide/

## What you see?

## Using TAB

## Going back on time
http://www.thegeekstuff.com/2008/08/15-examples-to-master-linux-command-line-history/#more-130

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

# FileSystem

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

/etc/gshadow` This file contains secure group account information.

# Basic Commands

## Navigation
`cd dirname` Moves you to the directory identified.

`mkdir dirname`	Creates the specified directory.

`ls dirname`	Shows the contents of the directory specified.

`cp file1 file2`	Copies one file/directory to specified location.

`mv file1 file2`	Moves the location of or renames a file/directory.

`rm filename`	Removes a file.

`rmdir dirname`	Removes a directory.

`df`

`du`

## Information 

`pwd`	Shows the current directory the user is in.

`file filename`	Identifies the file type (binary, text, etc).

`find filename dir`	Finds a file/directory.

`which filename`	Shows the location of a file if it is in your PATH.

`whereis filename`	Shows the location of a file.

`apropos`	Locate commands by keyword lookup

`info`	Displays command information pages online

`man`	Displays manual pages online

`whatis`	Search the whatis database for complete words.

`uname`		Display name of the current system

`users`		Print names of logged in users

`groups`	Show group memberships

`tty`		Print current terminal name

`stty`		Set terminal options

`who`		List logged in users

`w`			Show what logged in users are doing

`printenv`	Display value of a shell variable

##	Priviledges

`chwon`		Change owner

`chirp`		Change the group ownership of a file

`passed`	Change user password

`umask`		Show the permissions that are given to view files by default

## User manage

`useradd`	Adds accounts to the system.

`usermod`	Modifies account attributes.

`userdel`	Deletes accounts from the system.

`groupadd`	Adds groups to the system.

`groupmod`	Modifies group attributes.

`groupdel`	Removes groups from the system.

`last`		Show last logins of users

## Redirection Commands
Following is the complete list of commands which you can use for redirection:

`pgm > file`	Output of pgm is redirected to file

`pgm < file`	Program pgm reads its input from file.

`pgm >> file`	Output of pgm is appended to file.

`n > file`	Output from stream with descriptor n redirected to file.

`n >> file`	Output from stream with descriptor n appended to file.

`n >& m`	Merge output from stream n with stream m.

`n <& m`	Merge input from stream n with stream m.

`<< tag`	Standard input comes from here through next tag at start of line.
`|`			Takes output from one program, or process, and sends it to another.

## Process

`ps`		Report a snapshot of the current processes.

`top`		Display system tasks

`kill`		Send a signal to a process

`killall`

`htop`

`pstree`

`nice`/`renice`	Run a program with modified scheduling priority

`time`		Time a simple command or give resource usage

`uptime`	System Load Average

`bg` 	Place jobspec into the background, as if it had been started with `&'. If jobspec is not supplied, the current job is used.

`fg` 	Bring jobspec into the foreground and make it the current job. If jobspec is not supplied, the current job is used.

`jobs`	The first form lists the active jobs. The -l option lists process IDs in addition to the normal information; the -p option lists only the process ID of the job's process group leader. The -n option displays only jobs that have changed status since last notfied. If jobspec is given, output is restricted to information about that job. If jobspec is not supplied, the status of all jobs is listed.

`suspend`	Suspend the execution of this shell until it receives a SIGCONT signal. The -f option means to suspend even if the shell is a login shell.
When job control is active, the kill and wait builtins also accept jobspec arguments.

`screen`	http://www.ibm.com/developerworks/aix/library/au-gnu_screen/

# File Viewing/Editing

`echo`	Echo arguments to the standard options

`touch filename`	Creates a blank file or modifies an existing file.s attributes.

`cat filename` Displays a filename.

`head filename`	Shows the beginning of a file.

`tail filename`	Shows the end of a file.

`more filename`	Browses through a file from beginning to end.

`less filename`	Browses through a file from end or beginning.

`awk`	Pattern scanning and processing language

`cmp`	Compare the contents of two files

`comm`	Compare sorted data

`cut`	Cut out selected fields of each line of a file

`diff`	Differential file comparator

`expand`	Expand tabs to spaces

`join`	Join files on some common field

`perl`	Data manipulation language

`sed`	[Stream text editor](http://www.grymoire.com/Unix/Sed.html)

`sort`	Sort file data

`split`	Split file into smaller files

`tr`	Translate characters

`uniq`	Report repeated lines in a file

`wc`	Count words, lines, and characters

`fmt`	Simple text formatter

`vi`	Opens vi text editor

`vim`	Opens vim text editor

`emacs`	GNU project [Emacs](http://batsov.com/articles/2011/11/30/the-ultimate-collection-of-emacs-resources/) 

`pico`/`nano`	other editors 

# Compres

`compress`	Compress files

`gunzip`	Uncompress gzipped files

`gzip`	GNU alternative compression method

`uncompress`	Uncompress files

`unzip`	List, test and extract compressed files in a ZIP archive

`zcat`	Cat a compressed file

`zcmp`	Compare compressed files

`zdiff`	Compare compressed files

`zmore`	File perusal filter for crt viewing of compressed text

# Network Clients

`ftp`	File transfer program

`rcp`	Remote file copy

`rlogin`	Remote login to a UNIX host

`rsh`	Remote shell

`tftp`	Trivial file transfer program

`telnet`	Make terminal connection to another host

`ssh`	Secure shell terminal or command connection

`scp`	Secure shell remote file copy

`sftp`	secure shell file transfer program

# Network Tools

`ping`

`nslookup`

`netstat`	Print network connections, routing tables, interface statistics, masquerade connections, and multicast memberships

`finger`

`ifconfig`

`wget`

`rsync`

# Communication

`mail`	Simple send or read mail program

`mesg`	Permit or deny messages

`parcel`	Send files to another user

`pine`	Vdu-based mail utility

`talk`	Talk to another user

`write`	Write message to another user

# More sources

http://www.commandlinefu.com/commands/browse

http://everythingsysadmin.com/2012/09/unorthodoxunix.html

http://www.pixelbeat.org/cmdline.html



