# dotfiles

> Inspired by https://dotfiles.github.io/

Just need a place to organize my dotfiles

- GNU Stow is a good tool to symlink dotfiles dir and $HOME
	- `sudo apt-get install stow`
	- .stow-local-ignore like .gitignore
	- `stow --adopt .` would sync $HOME to dotfiles dir
		- to prevent accidentally commit secrets in $HOME, use `*` .gitignore
		- and `git add -f .X` to add a specific file

- .bashrc
- .vimrc
- .vim, theme
- .config
  - terminator, config and theme
