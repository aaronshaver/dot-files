# Make your macOS terminal and shell experience awesome.

## Install these programs.

Homebrew, a package manager for macOS: https://brew.sh/

iTerm2, a modern replacement for the default terminal: `brew cask install iterm2`

Make sure zsh is up to date: `brew install zsh`

Oh My Zsh, a framework for managing zsh: https://ohmyz.sh/

zsh-autosuggestions: `git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions`

powerlevel9k theme for zsh (installed oh-my-zsh style):

    git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k

tldr, a more useful alernative to man pages:

    npm install -g tldr

## Configure iTerm2.

1. Change the theme: first import the .itermcolors file (iTerm > Preferences > Profiles > Colors > Color Presets > Import), then switch to it
1. Install Powerline fonts (see the shell script code in the README): https://github.com/powerline/fonts
1. Change the font: iTerm > Preferences > Profiles > Text > 18pt Roboto Mono Medium for Powerline

## Commandline reference

### grep

recursive search in current directory: `grep search_term -r .`

### other

* Use vi mode in zsh: https://github.com/robbyrussell/oh-my-zsh/blob/master/plugins/vi-mode/README.md
* To run a Bash command: `bash -c <your command and args>`
* You can copy text into the macOS clipboard buffer by simply highlighting text with the mouse in iTerm2
* Re-run your last sudo command with `sudo !!`
* Get more useful help with tldr: `tldr <command>`
