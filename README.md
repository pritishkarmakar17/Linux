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

### ***tmux*** **essential codes**
- open tmux `tmux`
- tmux **prefix** changed to <kbd>Ctrl</kbd> + <kbd>a</kbd> from <kbd>Ctrl</kbd> + <kbd>b</kbd> (default) in  ~/.tmux.config.
- Panes management
    - create a new pane side-wise **prefix**, then <kbd>%</kbd>
    - create a new pane below **prefix**, then <kbd>"</kbd>
    - switch between the panes **prefix**, then <kbd>&uarr;</kbd>/<kbd>&darr;</kbd>/<kbd>&larr;</kbd>/<kbd>&rarr;</kbd>
    - change dimensions of pane **prefix** + <kbd>&uarr;</kbd>/<kbd>&darr;</kbd>/<kbd>&larr;</kbd>/<kbd>&rarr;</kbd>
    - exit pane `exit`
- Windows management
    - new window **prefix**, then <kbd>c</kbd>
    - list the window **prefix**, then <kbd>w</kbd>
    - switch between the window **prefix**, then <kbd>n</kbd> (n → window no.) or **prefix**, then <kbd>p</kbd>/<kbd>n</kbd>  (previous/ next)
    - rename window **prefix**, then <kbd>,</kbd> ,then rename it & **Enter**
- Sessions management
    - new session `tmux new -s <session_name>`
    - detach from session  **prefix**, then <kbd>d</kbd> (in session terminal)
    - view tmux session `tmux ls`
    - attach to a session  `tmux attach -t <n>` (<n> → session no)
    - rename session `tmux rename-session -t <old_name> <new _name>`  (initially `<old_name>` = `<n>)`
    - kill session `tmux kill-session -t <session_name>`
    

### ***Vim/  Neovim*** **essential codes** 
- open file in vim (neovim) `vim <file_name>` (`nvim <file_name>`)
- for help `:h <name>`
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
    - **Esc** - exit insert mode
- Editing
    - `u` - undo
    - `U` - restore (undo) the last changed line
    - **Ctrl + r** - redo
    - `.` - repeat the last command
- Visual commands
    - `y` - yank (copy) marked text
    - `d` - delete marked text
    - `~` - switch case
    - `u` - change marked text to lowercase
    - `U` - change marked text to uppercase
    - `v` - switch between normal and visual mode
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

### ***Git*** **essential codes**
- [Git CLI](https://github.com/pritishkarmakar17/Git_CLI)

### ***gcc*** **essential codes**

- make c file `touch new_file.c`, then open & edit it with any editor.
- compile the file `gcc new_file.c`(give default output **a.out** in that directory)
- compile the file with the new name `gcc -o output_file new_file.c`  (give output **output_file** in that directory) (`-o` output the file)
- run the file `~/path/of/the/output_file` or simply `./output_file`(if u r in same directory)
