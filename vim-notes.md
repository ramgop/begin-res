# Ram's Vim notes
This is intented to cheat sheet which can also be used to learn what I feel are the most useful aspects of vim.
  Note that anything with a `:` relates to a vim command, and unless otherwise specified all commands are from Normal Mode.
## The essentials
### Getting around
`/`                             - search. Pretty amazing to use to jump to places not just to search (n for next, N for previous)

`?`                             - reverse search (exactly same as search apart from N and n are swapped around)

`^`                             - go to start of line

`$`                             - go to end of the line

`hjkl`                          - left, down, right, up. Seriously amazing when you get it because no moving hands.

`w`                             - go forward one word

`b`                             - go to start of current word (or previous word if already at start)

`e`                             - go to end of the word

`ctrl + o`                      - go to the previous cursor position

`:help`                         - help is your friend. use `ctrl + ]` to follow links to sections

### Changing modes

`v`                             - go to visual mode

`ctrl + v`                      - go to visual block mode like ctrl + click on mouse based things (I use it lots for commenting code i.e. visually choose lines 
then add '#' 

`V`                             - go to visual line mode  (good for copying/moving blocks of lines)

`a`                             - Append. move cursor forward and change to Insert mode

`A`                             - go to end of line and change mode to Insert mode

`cw`                            - change word. i.e. delete word and change to Insert mode

### Selecting

note that a lot of these are actually changing modes and doing stuff but i consider these keyboard combinations more as words than individual 

#### Visual mode commands

`y`                             - yank (i.e copy)

`d`                             - delete (i.e cut)

`p`                             - paste after cursor

`P`                             - paste before cursor


#### Combo commands

`viwy`                          - Visual Inner Word Yank. i.e. select word and put it in buffer to paste

`viwp`                          - Visual Inner Word Paste. i.e. select word and paste someting over it (used with above command)

`:R"`                           - get whatever was last in buffer and put it in command area more useful as `:/R"` i.e. find what was yanked


### Replacing and deleting

`:%s/a/b/`                      - regex string replace (add g at end of command to allow multiple replacements per line.

`d$`                            - delete to the end of line

`dt<char>`                      - delete to character


### Tabs and Panes and files

`:tabnew <filename>`            - opens a new tab (note filename is optional

`vim -p <file1> <file2>`        - from command line, opens vim with multiple tabs

`gt`                            - Go To the next tab

`gT`                            - Go To the previous tab

`:split`                         - 

`:vsplit`

`ctrl+w w`

`:e <filename>`                 - edit file. can use '.' to browse files

ctrl +e ctrl-x edit command line command in vim
## More advanced
### Manipulating files

`:r`                            - reads a file and puts its contents in the buffer in the current position

`:!<cmd>`                       - executes a terminal command (it can be used with r like `:r!ls` to write output of command to buffer

### recording macros
### non-ascii


## Plugins
