# Emacs cheatsheet

## Notation
- C is the control key.  M is the meta or alt key.
- If your meta or alt key doesn't work, press and then release  <esc>.
- Key chords are combinations so  "C-h t" means press control and h at the same time, release, then press t
- For the embedded Emacs tutorial C-h t


## File Processing
    C-x C-f     open new file
    C-x C-v    open another file instead, in the same buffer
    C-x C-s    Save file
    C-x C-w   Save as and then type file name in mini buffer.  Same as "save as"
    C-x k       Close or "kill" current file
    C-g          Quit command.  This is great when you accidentally type the wrong command **
    C-x s       Save all modified files
    C-x C-c    Exit emacs


## Buffers
    C-x b   Switch buffer.  Press TAB to list all buffers
    C-x k   Kill current buffer


## Cursor Control
    C-f     forward one char
    C-b    back one char

    M-f     forward one word
    M-b    back one word

    C-n    next line
    C-p    previous line

    BACK      delete a char before cursor
    C-d       delete next char after cursor
    M-BACK    delete word before cursor
    M-d       kill word
    M-k       kill sentence
    C-k       kill to eol
    C-y       'yanks' the text back.  It reinserts text you killed. You can't yank text you deleted.
    M-y       Retyping this will yank earlier kills

    C-a   move to beginning of the line
    C-e   move to the end of the line
    M-a   move to the beginning of the sentence
    M-e   move to the end of the sentence

    C-u M-q   Aligns the current paragraph

    M-<   beginning of document
    M->   end of document

## Copy, Paste, Undo
You copy things in terms of blocks in Emacs.  You set a marker for the beginning of the block by pressing C-spacebar  or C-@, then move to the end of the block.

    M-w      copy
    C-w      cut
    C-y      paste

    C-/      undo.  You can also do C-x u, but / is easier.
    C-_      redo

    C-x h   select all


## Search & Replace
    C-s         search.  Press again for next occurrence.
    C-r         search previous or search backwards.  Type enter to cancel the search  
    C-g         return to starting point
    M-%         replace string
    C-q C-j     newline
    C-q C-m     carriage return


## Windows  
```
    C-x 2                   split into 2 windows
    C-x o                   Move to the (o)ther pane
    C-x 1                   1 window
    M-`                     Command line menus
    hold c + right click    popup menu
```

##  Help  
    C-h i           Info.  Enter to follow link.  Last page 'l', next section 'n', previous section 'p'
    M-x man         Man
    C-h t           Interactive tutorial
    C-h <command>   Tells you what <command> does


##  Numeric Arguments  
    C-u <number> <command>    Executes a command by a certain number

  Examples:
```
    C-u 8 C-n    Move down 8 lines  
    C-u 10 *       Print 8 asterisks

    C-x z   Repeat last command.  Works well with above examples.  To repeat more than once, type more z's
```


## Lisp editing
    M-/   self-insert

## SLIME  
    C-c C-c   compile defun
    C-c C-q   insert closing parens for all open parens

## Fancy Stuff  
    Append a file:  Move to end of file, then C-x i
