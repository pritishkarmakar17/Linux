# Linux
## Linux command lines

### **Directory management**

- change directories `cd /dir_name`
- go to previous directory `cd ..`
- print working directory `pwd`
- make directory  `mkdir <dir_name>` ( or `mkdir -p <dir_1>/<dir_2>`)
- remove empty directory `rmdir <dir_path>`
- delete the whole directory and anything within it `rm -r <folde_name>`  (recursively `-r`)
- tree structure of contents `tree`
- list their contents `ls` (`-l` for the long format, `-a` for hidden file )
- find file or directory `find <name>`

### ******************************File management******************************

- make file `touch output.<extension_name>` (e.g. `.py`, `.c`, `.cpp` etc)
- copy to directory `cp <filename> <to_directory_path>`
- move to directory `mv <filename> <to_directory_path>`
- rename `mv <output> <renamed_output>`
- word count in docs `wc -l combined.txt` (line count `-l`)
- brief description `file <filename>`
- file search `locate <filename>`
- view, open and edit files by nano `nano <file_name>`

### ****************************Terminal codes****************************

- print something `echo <something>`
- clear terminal `clear`
- command history `history`
- user id `id`
- username `whoami`
- change the user password `passwd`
- display tasks `top` or `htop`
- shutdown or reboot `shutdown`
- file download from website `wget <url>`
- open cli map `mapscii`
- generate text banner `figlet <text>'`

### **package-management**

- finding the package in the repository  `apt-cache search <search_string>`
- install packages  `apt-get install <package_name>`
- install package from package file `dpkg -i <package file>`
- remove package `apt-get remove <package_name>`
- update and upgrade packages `apt-get update`; `apt-get upgrade`
- list of installed packages `dpkg -l`
- package status `dpkg -s <package_name>`
- package file identification `dpkg -S <file_name>`


- ***tmux** essential codes:*
    - open tmux `tmux`
    - tmux **<prefix>** changed **Ctrl + a** to **Ctrl + b** (default) in  ~/.tmux.config.
    - Pane management
        - create a new pane side-wise <kbd>Ctrl</kbd> + <kbd>b</kbd> + `%`
        - create a new pane below <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `“`
        - switch between the panes <kbd>Ctrl</kbd> + <kbd>b</kbd>  + <kbd>&uarr;</kbd>/<kbd>&darr;</kbd>/<kbd>&larr;</kbd>/<kbd>&rarr;</kbd>
        - exit pane `exit`
    - Window management
        - new window <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `c`
        - list the window <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `w`
        - switch between the window <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `<n>` (<n> → window no.) or <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `p`/`n`  (previous/ next)
        - rename window <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `,`  ,then rename it & **Enter**
    - Session management
        - new session `tmux new -s <session_name>`
        - detach from session  <kbd>Ctrl</kbd> + <kbd>b</kbd>  + `d` (in session terminal)
        - view tmux session `tmux ls`
        - attach to a session  `tmux attach -t <n>` (<n> → session no)
        - rename session `tmux rename-session -t <old_name> <new _name>`  (initially `<old_name>` = `<n>)`
        - kill session `tmux kill-session -t <session_name>`
- ***Vim/  Neovim** essential codes:* ( [Vim cheatsheet](https://vim.rtorr.com/))
    - open file in vim (neovim) `vim <file_name>` `(nvim <file_name> )`
    - Cursor movement
        - `h` - move cursor left
        - `j` - move cursor down
        - `k` - move cursor up
        - `l` - move cursor right
        - `0` - jump to the start of the line
        - `$` - jump to the end of the line
        - `gg` - go to the first line of the document
        - `G` - go to the last line of the document (<n>gg or <n>G - go to line <n>)
        - `}` - jump to nextagraph (or function/block, when editing code)
        - `{` - jump to previous paragraph (or function/block, when editing code)
    - Inserting/ appending text
        - `i` - insert before the cursor
        - `I` - insert at the beginning of the line
        - `a` - insert (append) after the cursor
        - `o` - append (open) a new line below the current line
        - `O` - append (open) a new line above the current line
        - <kbd>esc</kbd>  - exit insert mode
    - Editing
        - `u` - undo
        - `U` - restore (undo) the last changed line
        - <kbd>Ctrl</kbd> + `r` - redo
        - `.` - repeat the last command
    - Visual commands
        - `y` - yank (copy) marked text
        - `d` - delete marked text
        - `~` - switch case
        - `u` - change marked text to lowercase
        - `U` - change marked text to uppercase
    - Cut and paste
        - `yy` - yank (copy) a line (`<n>yy` - yank (copy) <n> lines)
        - `dd` - delete (cut) a line (`<n>dd` - delete (cut) <n> lines)
        - `p` - put (paste) the clipboard after cursor
        - `P` - put (paste) before cursor
    - Indentation
        - `>>` - indent (move right) line one shiftwidth
        - `<<` - de-indent (move left) line one shiftwidth
    - Exiting
        - `:w` - write (save) the file, but don't exit
        - `:wq` or :x or `ZZ` - write (save) and quit
        - `:q` - quit (fails if there are unsaved changes)
        - `:q!` or `ZQ` - quit and throw away unsaved changes
        - `:wqa` - write (save) and quit on all tabs
    - Search & Replace
        - `/pattern` - search for pattern
        - `:%s/<old>/<new>/g` -replace all old with new throughout the file
        - `:%s/<old>/<new>/gc` -replace all old with new throughout the file with confirmations
- view, open and edit files by nano `nano <file_name>`
