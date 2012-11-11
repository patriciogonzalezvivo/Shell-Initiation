[![Header](https://raw.github.com/patriciogonzalezvivo/Shell-Initiation/master/images/terminal08.jpg)](http://patriciogonzalezvivo.com/)

In our journey we are in the point where we already know the terrain, now it time to start walking.

The fist tools you are going to use regularly are those for viewing files

*	`echo`				Echo arguments to the standard options

*	`touch FILENAME`	Creates a blank file or modifies an existing file.s attributes.

*	`cat FILENAME` 		Displays a filename.

*	`head FILENAME`		Shows the beginning of a file.

*	`tail FILENAME`		Shows the end of a file.

*	`more FILENAME`		Browses through a file from beginning to end.

*	`less FILENAME`		Browses through a file from end or beginning.

But viewing it's not enough. Isn't? Our terminal can act like a complete word processor. We will find that there are lot of programs that can process text.

*	`cmp`	Compare the contents of two files

*	`comm`	Compare sorted data

*	`cut`	Cut out selected fields of each line of a file

*	`diff`	Differential file comparator

*	`expand`	Expand tabs to spaces

*	`join`	Join files on some common field

*	`sort`	Sort file data

*	`split`	Split file into smaller files

*	`tr`	Translate characters

*	`uniq`	Report repeated lines in a file

*	`wc`	Count words, lines, and characters

*	`fmt`	Simple text formatter

*	`pico`/`nano`	Simple text editors 


Sometimes this is just not enough and you need to do heavy regular expressions stuff. You will find two incredible tools for that:

*	`awk`	Pattern scanning and processing language. Reference: [here](http://www.catonmat.net/blog/awk-one-liners-explained-part-one/)

*	`sed`	stream text editor. References: [here](http://www.pement.org/sed/sedfaq.html), [here](http://www.catonmat.net/blog/proof-that-sed-is-turing-complete/), [here](http://www.thegeekstuff.com/tag/sed-tips-and-tricks/), [here](http://tech.bluesmoon.info/2008/09/programming-patterns-in-sed.html) and [here](http://www.grymoire.com/Unix/Sed.html)

Intact `awk` and `sed` have there own kind of language. With is not strange to find in Unix contents. There are other unix programs that have their own language (script language) that you can use directly from the terminal. Must of them you already know them if you have been doing web work:

*	`perl`	

*	`python`

*	`php`

Even more, all the commands we have seen can be put together inside a file with a specify header and be executed by the the same program that let you type commands on your terminal (`bash`):

The header will specify witch program will use to execute the script.

	
	#!/bin/bash
	# Proper header for a Bash script.
	
or

	#!/usr/bin/python
	# Proper header for a Python script.
	
or

	#!/usr/bin/perl
	# Proper header for a Python script.

Little by little you are getting how close are the internet and UNIX. Isn't?
If you are interested on [How to Programming Bash Scritps check this link](http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO.html) of [this other one](http://linuxconfig.org/Bash_scripting_Tutorial)

You will find that this scripts not only have IF and FOR statements that you can use also on your terminal directly, but also the possibility to mix commands by passing through them information. This are call **pipes or redirections**. That mean you can *redirect* the out put of one command to be the input of other one.

[![Terminal Dorkshop](https://raw.github.com/patriciogonzalezvivo/Shell-Initiation/master/images/terminal07.png)](http://patriciogonzalezvivo.com/)

To do this plumbing magic you use the following simbols: 

*	`pgm > file`	Output of pgm is redirected to file

*	`pgm < file`	Program pgm reads its input from file.

*	`pgm >> file`	Output of pgm is appended to file.

*	`n > file`	Output from stream with descriptor n redirected to file.

*	`n >> file`	Output from stream with descriptor n appended to file.

*	`n >& m`	Merge output from stream n with stream m.

*	`n <& m`	Merge input from stream n with stream m.

*	`<< tag`	Standard input comes from here through next tag at start of line.

*	`|`			Takes output from one program, or process, and sends it to another.

You can found some [amazing examples of very useful lines that involve redirection here](http://www.commandlinefu.com/commands/browse)

Another important duty you are going to do on your terminal will involve not just moving files from here to there but also compress them and package them. For that there are this tools.

*	`compress`	Compress files

*	`uncompress`	Uncompress files

*	`gunzip`	Uncompress gzipped files

*	`gzip`	GNU alternative compression method

*	`unzip`	List, test and extract compressed files in a ZIP archive

*	`zcat`	Cat a compressed file

*	`zcmp`	Compare compressed files

*	`zdiff`	Compare compressed files

*	`zmore`	File perusal filter for crt viewing of compressed text

There is one that's particularly powerful that let you pack and compress in different formats call `tar` for witch is worth it to do a

	man tar
	
Speaking of power it's hard not to speak of two text editor that are SO incredible powerful that they can be use as IDEs and much more. This is the case of `vi` and `emacs` and the dived waters on their of developers choice. You can picture them as two doors to two different tribes. Choose wisely:

*	[Emacs](https://github.com/patriciogonzalezvivo/Shell-Initiation/blob/master/chap06a.md)

*	[Vi/vim](https://github.com/patriciogonzalezvivo/Shell-Initiation/blob/master/chap06b.md)