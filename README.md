# Make your terminal and shell experience awesome.

This document is oriented toward macOS users, though large parts of it will apply to *nix in general.

## Install these programs.

1. Homebrew, a package manager for macOS: https://brew.sh/
1. iTerm2, a modern replacement for the default terminal: `brew cask install iterm2`
1. Make sure zsh is up to date: `brew install zsh`
1. Oh My Zsh, a framework for managing zsh: https://ohmyz.sh/
1. zsh-autosuggestions: `git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions`
1. powerlevel9k theme for zsh (installed oh-my-zsh style): `git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k`
1. tldr, a more useful alernative to man pages: `npm install -g tldr`
1. tig, a better way to visualize Git history: `brew install tig`

## Configure iTerm2.

1. Change the theme: first import the .itermcolors file (iTerm > Preferences > Profiles > Colors > Color Presets > Import), then switch to it
1. Install Powerline fonts (see the shell script code in the README): https://github.com/powerline/fonts
1. Change the font: iTerm > Preferences > Profiles > Text > 18pt Roboto Mono Medium for Powerline

## General tips

* `dirs -v` in zsh lists the most recent 20 directories
* `%s/<your phrase>//gn` in Vim counts the number of matches for a search
* `terraform init <dir>` then `terraform plan <dir>` then `terraform apply <dir>` applies the Terraform .tf files for <dir>
* `go test -v ./...` recursively runs tests in a directory containing .go files
* `gra user@domain:<org name>/<project name>.git` adds an upstream remote to a Git config
* `top -o cpu` runs top sorting by most-CPU-usage first
* `tig` visualizes Git history in a better way
* `esc` and `i` on the commandline enters and exits vi-mode to edit your commandline
* To run a Bash command as it would run in Bash (instead of zsh): `bash -c <your command and args>`
* Get more useful help with tldr: `tldr <command>`
* You can copy text into the macOS clipboard buffer by simply highlighting text with the mouse in iTerm2
* `CTRL-U` clears the current line without sending a SIGINT as `CTRL-C` would do
* `grep search_term -r .` recursively searches for a string in files in the current directory

## oh-my-zsh Git plugin aliases

From: https://github.com/robbyrussell/oh-my-zsh/wiki/Plugin:git#aliases

* `gaa` git add --all
* `gba`	git branch -a
* `gc` git commit -v
* `gclean`	git clean -df (cleans uncommitted files only)
* `gcm`	git checkout master
* `gl` git pull
* `gpristine`	git reset --hard && git clean -dfx (cleans everything, including .gitignore files)
* `gpsup` git push --set-upstream origin $(current_branch)
* `gra` git remote add
* `gsb`	git status -sb
