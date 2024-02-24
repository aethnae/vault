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

