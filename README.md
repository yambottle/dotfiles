# dotfiles

> Inspired by https://dotfiles.github.io/

Just need a place to organize my dotfiles

## Notes
- GNU Stow is a good tool to symlink dotfiles dir and $HOME
	- `sudo apt-get install stow`
	- .stow-local-ignore like .gitignore
	- `stow -t $HOME .` would sync $HOME to dotfiles dir
		- to prevent accidentally commit secrets in $HOME, use `*` .gitignore
		- and `git add -f .X` to add a specific file
- TODO - find alternative for Mac
- TODO - checkout https://github.com/twpayne/chezmoi

## List of Files
- .bashrc
- .vimrc
- .vim, onedark theme
- .config
  - terminator, config and theme
- vscode
  - ~/.config/Code/User/, settings.json and keybindings.json
  - ~/.vscode/extensions/extensions.json 
- TODO - .zsh, oh-my-zsh, iterm2
