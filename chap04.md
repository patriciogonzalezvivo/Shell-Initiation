[![Terminal Dorkshop](https://raw.github.com/patriciogonzalezvivo/OldMysticSuperPowers/master/images/terminal06.png)](http://patriciogonzalezvivo.com/)

# File Viewing/Editing

`echo`	Echo arguments to the standard options

`touch FILENAME`	Creates a blank file or modifies an existing file.s attributes.

`cat FILENAME` Displays a filename.

`head FILENAME`	Shows the beginning of a file.

`tail FILENAME`	Shows the end of a file.

`more FILENAME`	Browses through a file from beginning to end.

`less FILENAME`	Browses through a file from end or beginning.

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

### Compres

`compress`	Compress files

`gunzip`	Uncompress gzipped files

`gzip`	GNU alternative compression method

`uncompress`	Uncompress files

`unzip`	List, test and extract compressed files in a ZIP archive

`zcat`	Cat a compressed file

`zcmp`	Compare compressed files

`zdiff`	Compare compressed files

`zmore`	File perusal filter for crt viewing of compressed text

[![Terminal Dorkshop](https://raw.github.com/patriciogonzalezvivo/OldMysticSuperPowers/master/images/terminal07.png)](http://patriciogonzalezvivo.com/)

# 8. Redirection Commands

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