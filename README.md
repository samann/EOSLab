# EOS LAB
## Brought to you by Spencer Amann

[Link for ViM tips](http://www.makeuseof.com/tag/5-things-need-put-vim-config-file/)

[Link for ViM Tutorial](https://danielmiessler.com/study/vim/#gs.yddGW34)


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
