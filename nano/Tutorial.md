# Nano

## Basics

Nano may be easier for quick editing, where it is installed on you server. It does not have modes, in other words it is always in editing mode. What you type becomes text. Instead it uses CTRL (C-) and  ALT (M-) to issue commands.

## Working with Files

Normally you start nano opening a file

nano Gerontion.md

but you can run nano and then open a file.

You open a buffer on the file.

C-O will save the buffer to file. It will prompt for the filename. C-T lets you use the file browser.
C-R appends a file into the current buffer. Again C-T lets you use the browser. M-F lets you append to a new buffer

## Editing

C-K Cut a line and C-U Paste a line
C-6 to begin selection, then C-K to cut and C-U to paste

## Searching

C-W to search (whereis) ALT+W to seatch again
But also exposes a sub-menu which lets you do things like goto line

## Configuration

There is a ~/.nanorc file

You can set variables, such as line numbers, softwrap of long lines etc.

If you clone this github repo, you can get syntax highlighting for a range of files

 




