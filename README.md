# mac-bootstrap
## Package Management
### Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```


## Terminal
### iterm2
```bash
brew install --cask iterm2
```

### zsh
```bash
brew install zsh
```

### ohmyzsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/andrewmadsen/.zprofile\n
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Version Control
```bash
brew install git
git config --global user.name "andrewrobertmadsen"
git config --global user.email "andrewrobertmadsen@gmail.com"
git config --global color.ui true
mkdir ~/.ssh && cd ~/.ssh
ssh-keygen -t rsa -C "andrewrobertmadsen@gmail.com"
chmod 400 id_rsa
pbcopy < ~/.ssh/id_rsa.pub #Add as new ssh key on github.
```
