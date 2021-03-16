# Getting started with Vim

Repo to document my journey to use Vim. 
It’s meant to be a personal documentation of the most important steps to get Vim (on Mac) working.

## Notes
On Mac there is a version of Vim installed already. However, it may not me the most current and some things don’t work (e.g. System Clipboard). To get the most current homebrew version of Vim use `brew install vim` resp. `brew upgrade vim`.

If preferred, you can map the Capslock key to ESC: https://vim.fandom.com/wiki/Map_caps_lock_to_escape_in_macOS

## Customizing Vim

> 📄 My .vimrc file can be found here: https://github.com/acsany/dotfiles

When you open Vim for the first time, it looks quite basic. By creating a `.vimrc` file (usually in your home-directory) and adding settings to it, you can customize it entirely.

Basic customizations may be:

```
set number                " show line numbers
set clipboard=unnamed     " use system clipboard

syntax on                 " Syntax highlighting
```

Type `:syntax on` to enable syntax highlighting.


## Commands (Normal Mode)
List of commands that I ~~used~~ had to look up first.

> You can combine counters with commands e.g. `2w` to jump *two* words forward.

### File commands
* **Save**: `:w`
* **Quit**: `:q`

### Adding/Deleting
* **Delete Line**: `dd`
* **Delete Word**: `dw`
* **Delete until end of line**: `d$`
* **Delete Character**: `x`
* **Add new line below**: `o`
* **Add new line above**: `O`

### Undoing
* **Undo previous action:** `u`
* **Undo all the changes on a line:**  `U`

### Navigation
* **Go to line number [n]**: E.g. `48gg`
* **Go to begining of line**: `0`
* **Go to end of line**: `$`
* **Go to beginning of next word**: `w`
* **Go to beginning of current/previous word**: `b`
