# Homebrew

Here is a list of commands I use frequently with [homebrew](https://brew.sh) on macOS.

## Create backup of Homebrew packages
```bash
cd /path/to/brewfile
brew bundle dump
```

## Restore backup from Brewfile
```bash
cd /path/to/brewfile
brew bundle install
```

## Upgrade everything
```bash
brew update && brew upgrade && brew upgrade --cask
```
