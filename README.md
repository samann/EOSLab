# EOS LAB
### Brought to you by Spencer Amann

## Bash
### Step one
    mkdir ~/bin && cd ~/bin

### Step two
    git clone https://github.com/samann/EOSLab.git

### Step three
    cp ~/.bashrc ~/bin/bash_test.sh
    
### Step four
    vim ~/bin/bash_test.sh
    
### Step five
    Modify the PS1 variable to change the prompt in a terminal window
    
### Variables
* \d : the date in "Weekday Month Date" format 
* \t : the current time in 24-hour HH:MM:SS format
* \w : the current working directory
* \s : the name of the shell
* \n : newline
* \\[ : begin a sequence of non-printing characters, for embedding a terminal control sequence into the prompt
* \\] : end a sequence of non-printing characters

### Color Codes

|   |   |
|---|---|
| 0;30m |  Black |
| 0;31m  | Red  |
| 0;32m  | Green  |
| 0;33m  | Yellow  |
| 0;34m  | Blue  |
| 0;35m  | Purple  |
| 0;36m  | Cyan  |
| 0;37m  | White  |

### Example PS1

```PS1="[\[\033[32m\]\w]\[\033[0m\]\n\[\033[1;36m\]\u\[\033[1;33m\]-> \[\033[0m\]"```

## Emacs
[Emacs Cheat Sheet](http://www.rgrjr.com/emacs/emacs_cheat.html)

#### task management
* C-h C-h : help
* C-g : quit
* C-x b : switch buffers
* C-x right : right-cycle through buffers
* C-x left : left-cycle through buffers
* C-x k : kill buffer

#### window management
* C-x 0 : close active window
* C-x 1 : close all windows except the active window
* C-x 2 : split the active window vertically into two horizontal windows
* C-x 3 : split the active window horizontally into two vertical windows
* C-x o : change active window to next window

#### file management
* C-x C-f : open file
* C-x C-s : save file
* C-x C-w : save file as

#### cut and paste text
* C-space : set region mark (starting point for text operation)
* C-w : kill region (cut text area)
* C-k : kill region between point and end of current line
* M-w : kill region without deleting (copy text area)
* C-y : yank region from kill ring (paste what was most recently cut/copied/killed)
* M-y : move to previous item in the kill ring
* M-Y : move to next item in the kill ring

* C-_ : undo

#### search functions
* C-s : search forwards
* C-r : search backwards
* M-% : query replace (‘space’ to replace, ‘n’ to skip, ‘!’ to replace all)
* M-q : wrap text

#### cursor movement
* C-p: move one line up
* C-n: move one line down
* C-f: move one character forward
* C-b: move one character backwards
* C-left : move one word left
* C-right : move one word right
* C-up : move one paragraph up
* C-down : move one paragraph down
* home : move to the beginning of the line
* end : move to the end of the line
* page up : move up a page
* page down : move down a page
* M- : move to end of buffer


## ViM
#### Vundle (ViM package manager)
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

set nocompatible

filetype off

set rtp+=~/.vim/bundle/Vundle.vim

call vundle#begin()

Plugin 'VundleVim/Vundle.vim'

call vundle#end()

filetype plugin indent on

