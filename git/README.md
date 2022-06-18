# git

## Add Global Config 
```
git config --global include.path ~/dotfiles/git/.gitconfig_global
```

## Add Local Config in Repo
use `Makefile`
```
init:
	cp ~/dotfiles/git/.gitconfig_local .gitconfig_local
	git config --local include.path ../.gitconfig_local
	git config --local --list
```
