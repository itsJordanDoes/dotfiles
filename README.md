# Ohmyzsh
```sh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

# Homebrew
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
# GH CLI
```sh
brew install gh
gh auth login
```

# Brewfile
```sh
# clone this directory and then install brewfile
gh repo clone itsJordanDoes/dotfiles
cd dotfiles
brew bundle install ./Brewfile
```

# Link up stuff
```sh
ln -Fs dotfiles/zshrc .zshrc
ln -Fs dotfiles/nvimrc .nvimrc
ln -Fs dotfiles/vimrc .vimrc
ln -Fs dotfiles/tmux.conf .tmux.conf
ln -Fs dotfiles/gitconfig .gitconfig
ln -Fs ~/dotfiles/alacritty.yml ~/.config/alacritty/alacritty.yml
ln -F ~/dotfiles/settings.json ~/Library/Application\ Support/Code/User/settings.json

cp dotfiles/aliases.zsh $ZSH_CUSTOM/aliases.zsh
source ~/.zshrc
```

# Download and setup theme
```sh
curl https://raw.githubusercontent.com/therealklanni/purity/master/purity.zsh --output purity.zsh
ln -s purity.zsh ~/.oh-my-zsh/themes/purity.zsh-theme
```

# Neovim
```sh
brew install neovim
#  Install vim-plug
curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

# tmux
```sh
# Install tpm for tmux plugins
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
ln -s dotfiles/tmuxline ~/.tmux/tmuxline
```


# Node / nvm / npm
```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
```

# Mac Stuff
```sh
# Remove Dock Animation
defaults write com.apple.dock autohide-time-modifier -float 0;killall Dock
defaults write com.apple.dock autohide-delay -float 0; killall Dock
defaults write com.apple.dock workspaces-swoosh-animation-off -bool YES
defaults write com.apple.finder AppleShowAllFiles -bool YES
 New Screenshots folder
mkdir ~/Documents/Screenshots
defaults write com.apple.screencapture location ~/Documents/Screenshots
```
