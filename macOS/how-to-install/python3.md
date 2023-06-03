* Rev.1: 2023-06-03 (Sat)
* Draft: 2021-12-30 (Thu)

# How to Install Python3 on macOS

## Overview
* To use Python3 on macOS, install it separately because Python2 is the default Python version on MacOS.
```bash
$ python --version
Python 2.7.18
$
```
* If you need multiple Python versions, use `pyenv` which lets you easily switch between multiple versions of Python. For details, refer to [Simple Python Version Management: pyenv](https://github.com/pyenv/pyenv).
```bash
$ brew install pyenv
$
```
* If you need to install Python3 for Google Cloud, refer to **Google Cloud > Python > Documentation > Guides > Setting up a Python development environment > [Installing Python](https://cloud.google.com/python/docs/setup#installing_python)**.

## Prerequisite: install `brew` first
* Homebrew or `brew` is a package manager for macOS and Linux.
* 'brew' is not pre-built on macOS. 
* So install `brew` first.
* Refer to [How to Install Homebrew or brew on macOS](https://github.com/aimldl/computing_environments/blob/main/macOS/how-to-install/brew.md).

## Install `python3` via `brew`
```bash
$ brew install python
```

## Verify the installation
```bash
$ brew list | grep python
python@3.9
$
```
or
```bash
$ python3
Python 3.7.9 (v3.7.9:13c94747c7, Aug 15 2020, 01:31:08) 
[Clang 6.0 (clang-600.0.57)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> exit()
$
```

## References
* [Installing Python 3 on Mac OS X](https://docs.python-guide.org/starting/install3/osx/), The Hitchhiker's Guide to Python
* [Simple Python Version Management: pyenv](https://github.com/pyenv/pyenv)
* Google Cloud > Python > Documentation > Guides > Setting up a Python development environment > [Installing Python](https://cloud.google.com/python/docs/setup#installing_python)
* [How to Install Homebrew or brew on macOS](https://github.com/aimldl/computing_environments/blob/main/macOS/how-to-install/brew.md)
