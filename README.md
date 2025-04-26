# dotfiles

> Inspired by https://dotfiles.github.io/

Just need a place to organize my dotfiles

## Notes
- GNU Stow is a good tool to symlink dotfiles dir and $HOME
  - Linux: `sudo apt-get install stow`
  - Mac: `brew install stow`
- Config
  - .stow-local-ignore like .gitignore
  - `stow -t $HOME .` would sync $HOME to dotfiles dir
  - to prevent accidentally commit secrets in $HOME, use `*` .gitignore
	- and `git add -f .X` to add a specific file
- TODO - checkout https://github.com/twpayne/chezmoi

## List of Files
- .bashrc
- .zshrc
- .oh-my-zsh
  - eastwood theme with added timestamp
- .vimrc
- .vim
  - onedark theme
- .config
  - terminator, config and onedark theme
- ~~vscode, cursor~~ comes with 'setting sync'

## A Bit Toil Is Fine
> Not synced by `stow` but good to have
- iterm2
    - Settings -> Profile -> default -> Keys -> Key bindings -> Preset -> Natual Text Editing
    - OneDarkPro Theme
      - `curl -o OneDarkPro.itermcolors https://raw.githubusercontent.com/chinhsuanwu/one-dark-pro-iterm/master/One%20Dark%20Pro.itermcolors`
      - Settings -> Profile -> Colors -> Color Preset -> Import above file 


