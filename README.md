# dwmblocks

Modular status bar for dwm written in c (from lukemsithxyz)

# Modifying blocks

The statusbar is made from text output from commandline programs.  Blocks are
added and removed by editing the config.h file.


codeblocks for each commands is stored in .local/bin
and added to 
`$PATH`.
by `export PATH="$HOME/.local/bin:$PATH"`


#extra
For example, the audio module has the update signal 10 by default.  Thus,
running `pkill -RTMIN+10 dwmblocks` will update it.

You can also run `kill -44 $(pidof dwmblocks)` which will have the same effect,
but is faster.  Just add 34 to your typical signal number.



Note that all modules must have different signal numbers.
