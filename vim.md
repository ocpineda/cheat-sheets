## File Handling

`:q!`   quit without saving  
`:w`    save  
`:wq`   save and quit  
`:!`    &lt;command&gt; execute an external command.  

## Cursor movement
`gg`      go to beginning of file  
`G`       go to end of file  
`0`       move to start of line  
`$`       move to end of line  
`w`, `W`  next word  
`b, B `   previous word
`w,W`     jump to start of words, jump word spaces

## Matching >, ], or }

% Jump to matching bracket, paren, brace, less than sign.

## Editing
```
u undo last command

U undo line

Ctl-R redo

x delete char

i, a insert before, or after cursor

I, A insert before, or after a line

p puts previously deleted line in front of cursor. When used with dd it works like cut and

paste

d2w delete two words

dd. D delete a line

2dd delete two lines

r replace, then type the char that should be there

ce change until the end of the word

cw change word

c$ change to end

o,O open a new a new line below the cursor, open above the cursor
```


## using a count as a motion and delete
`<number>w` ex: 2w move two words

## Search
/ to search a phrase

? search for occurrence

n for next, N for previous occurrence

Ctl-o go back to last cursor placement

Ctl-i goes forward instead

The Substitute Command (search and replace)

:%s/foo/bar/g find all foo and replace it with bar

:%s/foo/bar/gc find all foo and replace, but ask for confirmation

:%s/foo/bar/gci case sensitive find and replace with confirmation

:s/foo/bar/g replace all foo with bar in the current line

## Cursor Movement
Ctrl-G show cursor placement

<num>G go to line number

{ begin para

} end para

page up/down Ctrl+U, Ctrl+D

gk line up

gj line down

## Visual Mode

v, V highlight one character at a time, block at a time.
