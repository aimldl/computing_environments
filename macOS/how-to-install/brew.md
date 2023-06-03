* Rev.1: 2023-06-03 (Sat)
* Draft: 2021-12-15 (Wed)

# How to Install Homebrew or `brew` on macOS
* Homebrew is a package manager for macOS and Linux.
* You don’t need `sudo` after Homebrew’s initial installation when you `brew install`.

## Install
Google search: mac how to install brew
* Homebrew Documentation > Installation > [Git Remote Mirroring](https://docs.brew.sh/Installation#git-remote-mirroring)

Open Terminal and run the following commands.
```bash
$ export HOMEBREW_BREW_GIT_REMOTE="..."  # put your Git mirror of Homebrew/brew here
$ export HOMEBREW_CORE_GIT_REMOTE="..."  # put your Git mirror of Homebrew/homebrew-core here
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

The necessary interaction to proceed the installation is below.
First, enter the password.
```bash
==> Checking for `sudo` access (which may request your password)...
Password: 
```
Press `Enter`.
```bash
  ...
Press RETURN/ENTER to continue or any other key to abort:
```
and wait ...
```bash
  ...
Software Update Tool

Finding available software

Downloading Command Line Tools for Xcode
```
## Verify the installation
```bash
$ which brew
/usr/local/bin/brew
$
```
or
```bash
$ brew help
Example usage:
  ...
$
```

## Example usage
```bash
$ brew help
Example usage:
  brew search TEXT|/REGEX/
  brew info [FORMULA|CASK...]
  brew install FORMULA|CASK...
  brew update
  brew upgrade [FORMULA|CASK...]
  brew uninstall FORMULA|CASK...
  brew list [FORMULA|CASK...]

Troubleshooting:
  brew config
  brew doctor
  brew install --verbose --debug FORMULA|CASK

Contributing:
  brew create URL [--no-fetch]
  brew edit [FORMULA|CASK...]

Further help:
  brew commands
  brew help [COMMAND]
  man brew
  https://docs.brew.sh
$
```

## What is Homebrew or `brew`?
> Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's operating system, macOS, as well as Linux. The name is intended to suggest the idea of building software on the Mac depending on the user's taste.
- source: [Homebrew (package manager)](https://en.wikipedia.org/wiki/Homebrew_(package_manager))

***People also ask*** > Is brew and Homebrew same?
> brew is the core command for the Homebrew project. Homebrew installs the stuff you need that Apple didn't. Homebrew typically deals with command line software (not graphical GUI applications). Most of the software is distributed under an open source licence.Sep 25, 2017
- source: [What is the difference between brew install X and brew cask install X](https://stackoverflow.com/questions/46403937/what-is-the-difference-between-brew-install-x-and-brew-cask-install-x#:~:text=brew%20is%20the%20core%20command%20for%20the%20Homebrew%20project.&text=Homebrew%20installs%20the%20stuff%20you,under%20an%20open%20source%20licence.)
