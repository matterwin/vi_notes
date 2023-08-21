# vi_notes

# how to quit vim/vi
:q! or just :q or just shift twice Z

# :q! 
quits out the file without regard to saving your unsaved changes


# how to write something:
when we enter vim, we enter a normal mode (so rn in the perspective of normal mode)

# : key 
starts a command like :q

# i 
goes into insert mode and insert mode is just text that you type

# esc key 
exits insert mode

# :w 
writes the file or it is saved to the file

# :wq
writes to the file and quits vi

# a and o
can enter the insert mode but the way cursor operates is different

# in insert mode via i
you enter chars before the cursor or on the LHS of the cursor or just like a regular windows cursor

# a
goes into insert mode and every char is put on where the cursor is

# o
goes into insert mode, but it creates a newline below the cursor of where and when you pressed o

# I or shift + i
puts cursor at the beginning of the line in insert mode of course

# A or shift + a
puts cursor at the end of the line in insert mode of course

# O or shift + o
puts cursor above of the line in insert mode of course

# :set numbers or :set nu
to have line numbers in your editor

# :set wm
word wraps the text

numbers can be used to combine keybindings

# # + arrow key down or up or left or right
moves your cursor down or whatever by # lines in normal mode
example 5 + key down moves cursor down 5 lines 

can just jkhl key for up, down, left, right

# :set relativenumber
changes the line numbers based on the position of the cursor
this setting can be combined with pacing and deletion, but its more advanced and weird

# :set mouse=a
you can use mouse and scroll like normal with mouse

# :set tabstop=4
# :set shiftwidth=4
# etc

# :colorscheme <tab> to see color schemes

all settings are gone if you leave the file, and so go to this
# vi ~/.vimrc

and add your settings there

# esc + d twice
deletes whole line where cursor is at in insert mode
or in normal mode

# d twice
deletes whole line where cursor is at in normal mode

# D or shift + d
deletes everything right of the cursor on the same line in normal mode

# :w filename.txt
performs a "save as" operation and will save your changes as a new file

# diff myfile.text mynewfile.txt
linux cmd that tells you the difference btw the files and will show the diff lines

to move around the file you must always be in normal or command mode (same thing)

two diff cmds to perform a search

# /sample
will show the pattern matched from what you typed to what's found in the file and you must be in normal mode
forward direction (meaning it'll find the match after where your cursor is)

# ?sample
backward direction (meaning searches behind or LHS of cursor and above)

# N
for forward direction traversal through file

# n
for backward direction traversal through file

# special chars must be preceded by \

# / \n
searches for new lines in file
