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