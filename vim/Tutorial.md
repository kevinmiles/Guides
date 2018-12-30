#Vim

What you wanted to use EMACS? Heretic.

## Basic usage

### Editing a file

    vim The_Love_Song_Of_J_Alfred_Prufrock.md

#### Motions

    hjkl for moment also cursor keys
    w and b for words
    l next letter
    e next end of a word
    ge previous end of a word
    nw and nb for moving more than one word at a time
    fh Find h Th To h
    0 for beginning of line $ for end of line 
    ^ for first non-whitespace
    () for moving sentences
    {} for moving paragraphs
    m Bookmark
    ma create a Bookmark a
    ‘ jump to a bookmark
    ‘a jump to bookmark a
    :delmarks a delete bookmark a
    `` jump back (two back-ticks)
    1G First Line. 50G 50th line
    G EOF
    1 CTRL-B One page back 1 CTRL-F One page forward
    CTRL U Scroll up CTRL D scroll down
    CTRL-G Where am I?
    zz move line under cursor to the middle of the screen

 #### Edit Modes

    Insert and Normal Mode. Using ESC to toggle between the two
    i turn on Insert Mode. ESC turn on normal mode
    a append
    SHIFT a append at end of line
    c change
    cw change word
    c3l change 3 letters
    x delete character
    d delete
    dl delete letter, dw delete word
    d3w delete 3 words
    dd delete line
    u undo
    p paste. The paste buffer will contain the last thing deleted, but default
    y yank i.e. copy
    yw copy word
    y3w copy 3 words
    v select
    Example 0v 2j
   >> indent << unindent
    How to save :w (or :wa for all buffers)
    How to quit: :q and :q!

### Opening and Closing Files

    :edit my file.txt Open or create the file my file.txt (must not have unsaved changes)
    : ls or :buffers list the buffers
    [Note the + symbol by a dirty buffer]
    :b N switch to buffer

## Advanced Usage

### Splitting the Window

   :split Splits the window at the cursor
   :split my file.txt Splits the window and opens the file
   :new splits new window with an empty file in it 
   :vsplit vertical instead of horizontal split
   :vnew splits vertically with new empty file 
   :close closes the current window (:q works but risks closing the editor)
   CTRL-W Switch between windows

### Tabs
    :tab edit my file.txt
    :tabc close
    :tabn next tab
    :tabp previous tab

    N.B. Tabs should not be used like tabs in other IDEs i.e. one file per tab. A tab is really a layout i.e. a collection of windows over buffers. What is a window then? A window is a viewport onto a buffer. You can switch which buffer a window is the viewport of by using :bN
Preparefer to use buffers over tabs, until you grok the difference.

###  Searching
    / regex / find the pattern
    n next match

## Running Shell Commands
    Use :!{cmd} to run a command i.e. :! git status

## Cheat Sheet
    http://www.viemu.com/vi-vim-cheat-sheet.gif

## Configuring
  This is really fo when you want to use Vim as your IDE. Don’t rely on the plugins here. At some point you are going to need to SSH onto a vanilla Linux box and use Vim directly to edit, and you may not have the time to configure your .vimrc file and plugins, just the way that you want them. So you need to learn how to use basic Vim; reserve this stuff for wanting to use Vim as your IDE as opposed to a text editor.
   VimScript lets you configure the IDE
   You can type VimScript commands in normal mode
    :set number — turn on line numbers
    :set showmode - show the current mode
    But its more common to edit your vimrc
    The vimrc file: used to set all your options persistently, so you don’t need to set them up each time.
    Lives at ~/.vimrc
    You can just use something like spf-13 to get a set of defaults, particularly when you are learning
        : https://github.com/spf13/spf13-vim

## Plugins
    You can use plugin managers to load plugins into the IDE to improve capabilities
    There are a number of different plugin managers to make working with plugins easier: Vimplug, Vundle, NeoBundle and Pathogen are popular
    NERDTree (installed in the spa-13 package) gives you a file browser
    :NERDTree, opens NERD Tree
    :NERDTreeToggle switches it on and off
    :NERDTreeFind opens it with the current file
    :NERDTreeClose close the current NERDTree  
    Once inside the NERDTree
    <CR> or o is open file, directory
    s open in a new split
    I toggle hidden files
    Omnisharp: Omnisharp provides C# intellisense to Vim via the Rosyln compiler.
    https://www.palladiumgames.net/unity-development-with-vim-and-git-in-windows-part-2/
    You need msbuild installed etc. to make this work
 


    
    

     
