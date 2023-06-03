* Draft: 2021-12-15 (Wed)

# How to Install Homebrew or `brew` on macOS

## What is Homebrew or `brew`?
* Homebrew is a package manager for macOS and Linux.

> Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's operating system, macOS, as well as Linux. The name is intended to suggest the idea of building software on the Mac depending on the user's taste.
source: [Homebrew (package manager)](https://en.wikipedia.org/wiki/Homebrew_(package_manager))

***People also ask*** > Is brew and Homebrew same?
> brew is the core command for the Homebrew project. Homebrew installs the stuff you need that Apple didn't. Homebrew typically deals with command line software (not graphical GUI applications). Most of the software is distributed under an open source licence.Sep 25, 2017
source: [What is the difference between brew install X and brew cask install X](https://stackoverflow.com/questions/46403937/what-is-the-difference-between-brew-install-x-and-brew-cask-install-x#:~:text=brew%20is%20the%20core%20command%20for%20the%20Homebrew%20project.&text=Homebrew%20installs%20the%20stuff%20you,under%20an%20open%20source%20licence.)

## Summary
```bash
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
$ which brew
$ brew help
$
```

## Google search: mac how to install brew

### Install `brew` with Bash
```bash
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
The messages are below. Enter the root password.

```bash
==> Checking for `sudo` access (which may request your password)...
Password: 
==> This script will install:
/usr/local/bin/brew
/usr/local/share/doc/homebrew
/usr/local/share/man/man1/brew.1
/usr/local/share/zsh/site-functions/_brew
/usr/local/etc/bash_completion.d/brew
/usr/local/Homebrew

Press RETURN to continue or any other key to abort:
```
Hit enter.
```bash
  ...
==> Installation successful!

==> Homebrew has enabled anonymous aggregate formulae and cask analytics.
Read the analytics documentation (and how to opt-out) here:
  https://docs.brew.sh/Analytics
No analytics data has been sent yet (nor will any be during this install run).

==> Homebrew is run entirely by unpaid volunteers. Please consider donating:
  https://github.com/Homebrew/brew#donations

==> Next steps:
- Run brew help to get started
- Further documentation:
    https://docs.brew.sh
$
```
### Verify the installation
```bash
$ which brew
/usr/local/bin/brew
$
```

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

### The Ruby command is deprecated.
I don't recommend to use the following ruby command because
1. it took several tens of minutes on my newest macOS Pro and
2. installing Homebrew with Ruby is deprecated as follows:

```
Warning: The Ruby Homebrew installer is now deprecated and has been rewritten in
Bash. Please migrate to the following command:
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Command to install `brew` with Ruby
[Installing Homebrew on a Mac](https://treehouse.github.io/installation-guides/mac/homebrew) > Installation Steps

```bash
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
