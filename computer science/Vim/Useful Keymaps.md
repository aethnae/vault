---
tags:
  - vim
  - neovim
  - terminal
  - shell
flashcard: false
publish: false
source: :Tutor
aliases:
  - Hotkeys
  - Keymaps
date created: Saturday, February 24th 2024, 2:40:11 am
date modified: Saturday, February 24th 2024, 2:40:23 am
---
***

*This page serves as an overview & reference for commonly used **nvim** keymaps.*

***
#### Moving around

- `h`, `j`, `k` & `l` to move around

> [!tip] Useful motions for navigating in a file 
> Remember that pressing a *motion* while in **Normal mode** without an operator will move the cursor as specified.
> 
> Here are some useful motions:
> - `w` will move to the **start** of the next word, **excluding** its first character
> - `e` will move to the **end** of the next word, **including** its last character
> - `$` will move to the end of the line, **including** the last character

***
#### Exiting Neovim

- To exit Neovim, type
	- `<Esc> :q! <Enter>` to trash all changes
	- `<Esc> :wq <Enter>` to save the changes

***
#### Deleting, Inserting & Appending Text

- `x` to delete the character at the cursor
- `i` to enter **insert mode** *before* the cursor
- `A` to append text *after* the line

> [!note] Normal mode 
> Pressing `<Esc>` will place you in **Normal mode** or will cancel an unwanted and partially completed command.

***
#### Change Commands

> [!info] Change commands 
>The format for a change command is:
>
operator   [number] motion
> 
> where
> 
> - **operator** - what to do, such as `d` for *delete*
> - [number] - optional count to repeat the motion
> - motion - moves over the text to operate on, such as
> 	- `w` (word)
> 	- `$` (to the end of the line)

- To delete a *whole* line, type `dd`
- To move to the start of the line, use a zero `0`

***
#### Undo Commands

- To undo previous actions, type `u`
- To undo **all** the changes on a line, type `U`
- To undo the undo's, type `C-r` (command - r)

***
#### The Put Command

> [!info] Putbacks 
> To put back text that has just been *deleted*, type `p`. This puts the deleted text **after** the cursor.

- If a whole line was deleted, it will appear on the line under the cursor position

***
#### The Replace Command

- To replace the character under the cursor, type `r` and then the character you want to have there
- Typing a capital `R` enters Replace mode until `<Esc>` is pressed

***
#### The Change Command

> [!info] Change Operators
> The **change operator** allows you to change from the cursor to where the motion takes you.  Type `ce` to change from the cursor to the end of the word, `c$` to change to the end of a line, etc.

The format for change is:

**c**    [number]    motion

***
#### Cursor Status and Navigation

- `<Ctrl> g` displays your location and the file status
- `G` moves to the end of the file
- `[line number] G` moves to that line number
- `gg` moves to the first line

To search for specified terms, use these commands

- `/` followed by a phrase searches **forward** for that phrase
- `?` followed by a phrase searches **backwards** for that phrase
	- After a search, type `n` to find the next occurence in the same direction
	- `N` works the same, but searches in the opposite direction
- `<Ctrl> o` takes you back to older positions
- `<Ctrl> i` takes you to newer positions, when currently on an older position

> [!note] Bracket Search 
> Typing `%` while the cursor is on a (, ), [, ], { or } goes to its match.

***
#### Substitution

- To substitute "new" for the first "old" in a line, type `:s/old/new`
- To substitute "new" for all "old" on a line, type `:s/old/new/g`
- To substitute phrases between two line **#'s**, type `:#,#s/old/new/g`
- To substitute all occurrences in the file, type `:%s/old/new/g` 
	- To ask for confirmation each time add 'c', and type `:%s/old/new/gc`

***
#### Visual Selection

> [!info] Visual selection 
> Pressing `v` starts **visual selection**. You can move the cursor around to make the selection bigger or smaller. Then you can use an operator to do something with the text. For example, `d` deletes the text.

The format for visual selection commands is as follows:

`v`    motion    operator

***
#### Using External Commands

- `:!command` executes an external command
- Some useful examples are
	- `:!ls` shows a directory listing
	- `:!rm FILENAME` removes file FILENAME

***
#### Writing and Retrieving Files

- `:w FILENAME` writes the current Neovim file to disk with name FILENAME
- `:r FILENAME` retrieves disk file FILENAME and puts it **below** the cursor position
	- `:r !dir` reads the output of the `dir` command and puts it **below** the cursor position

***
#### Opening new Lines

- Type `o` to open a line **below** the cursor and start insert mode
- Type `O` to open a line **above** the cursor and start insert mode

***
#### Appending Text

- Type `a` to insert text **after** the cursor
- Type `A` to insert text after the end of the line

***
#### Yanking & Putting Text

> [!info] Copy & Paste
>  The `y` operator copies text, `p` pastes it.

***
#### Changing Settings

> [!info] The "set" Command 
> Typing `:set xxx` sets the option "xxx". Some options are
> - `ic`, short for `ignorecase` - ignore upper/lower case when [[Useful Keymaps#Cursor Status and Navigation|searching]]
> - `is`, short for `incsearch` - show partial matches for a search phrase
> - `hsl`, short for `hlsearch` - highlight all matching phrases

- You can either use the short or long option name
- Prepend `no` to switch an option off
	- For example, `:set noic` switches ignore case off
- Prepend `inv` to invert an option

***
#### Command Line Completion

- While in command mode, press `<Ctrl> d` to see possible completions
	- Press `<Tab>` to use one completion

***
#### Startup Scripts

> [!info] init.vim 
> Create an `init.vim` file to configure the startup behavior of nvim. For information about possible content, type `:help init.vim`

