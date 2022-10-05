# home

## Terminal configuration

[Install iTerm](https://www.iterm2.com)

### Install git
```
git version
```
Follow GUI instructions

### Install brew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
Or visit [brew.sh](https://brew.sh/)

### Install gh
```
brew install gh
```

### Install git autocomplete
```
brew install git bash-completion
```

### Install oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Install zsh plugins
```
brew install zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### Install custom agnoster theme (with time)
Copy [lima-agnoster.zsh-theme](https://gist.github.com/ccanete/cd3b20a0311b9fbbe7987008a90560d2#file-lima-agnoster-zsh-theme) to zsh themes folder `~/.oh-my-zsh/themes/`

### Restore .zshrc
```
rm ~/.zshrc
mv <path_to_dir>/home/.zshrc ~/.zshrc
```

### Install Fonts
[Download the font archive](https://github.com/powerline/fonts/archive/master.zip), and unzip it. Go to fonts-master/UbuntuMono/ and install each of the four TTFs.  

### Restore iTerm params
```
rm ~/Library/Preferences/com.googlecode.iterm2.plist
mv <path_to_dir>/home/com.googlecode.iterm2.plist ~/Library/Preferences/com.googlecode.iterm2.plist
```
restart iTerm

### Configure fonts in iTerm
1. Open Terminal, then navigate to Terminal Preferences > Profiles > Font and click the Change button.  
2. Select Ubuntu Mono derivative Powerline and set the font size to 14.  
3. Close preferences, and quit Terminal.

## Configure SSH defaults

Exemple
```
> cat ~/.ssh/config
HOST *.apple.co
     USER root
     IdentityFile ~/.ssh/apple
```

## Switch between windows of the same app

Go to Settings > Keybord > Shortcuts > Keybord  
Set **Move focus to the next windows** to `⌘@`

<img src="https://i.stack.imgur.com/P5MJ5.png" />
