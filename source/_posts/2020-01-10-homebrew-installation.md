---
title: Homebrew Installation
date: 2020-01-10 18:34:54
categories:
  - HomeBrew
tags:
  - HomeBrew
  - Brew
  - Terminal
  - Packet Manager
cover: https://i.ibb.co/kD9q6N4/mac-for-hackers-set-up-homebrew-install-update-open-source-tools-1280x600.jpg
---

## Installation
Instructions for a supported install of Homebrew are on the [homepage](https://brew.sh/).



This script installs Homebrew to /usr/local so that [you don’t need sudo](https://docs.brew.sh/FAQ#why-does-homebrew-say-sudo-is-bad) when you brew install. It is a careful script; it can be run even if you have stuff installed to /usr/local already. It tells you exactly what it will do before it does it too. You have to confirm everything it will do before it starts.

## Requirements
* A 64-bit Intel CPU
* macOS High Sierra (10.13) (or higher)
* Command Line Tools (CLT) for Xcode: `xcode-select --install`, [developer.apple.com/downloads]() or [Xcode](https://itunes.apple.com/us/app/xcode/id497799835)
* A Bourne-compatible shell for installation (e.g. bash or zsh)

## Untar anywhere
Just extract (or `git clone`) Homebrew wherever you want. Just avoid:
* Directories with names that contain spaces. Homebrew itself can handle spaces, but many build scripts cannot.
* `/tmp` subdirectories because Homebrew gets upset.
* `/sw` and `/opt/local` because build scripts get confused when Homebrew is there instead of Fink or MacPorts, respectively.

However do yourself a favour and install to `/usr/local`. Some things may not build when installed elsewhere. One of the reasons Homebrew just works relative to the competition is because we recommend installing to `/usr/local`. Pick another prefix at your peril!

```shell script
mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip 1 -C homebrew
```

## Multiple installations
Create a Homebrew installation wherever you extract the tarball. Whichever `brew` command is called is where the packages will be installed. You can use this as you see fit, e.g. a system set of libs in `/usr/local` and tweaked formulae for development in `~/homebrew`.

## Uninstallation
Uninstallation is documented in the [**FAQ**](https://docs.brew.sh/FAQ).

1. For 32-bit or PPC support see [Tigerbrew](https://github.com/mistydemeo/tigerbrew).
   
2. 10.13 or higher is recommended. 10.9–10.12 are supported on a best-effort basis. For 10.4-10.6 see [Tigerbrew](https://github.com/mistydemeo/tigerbrew).
   
3. Most formulae require a compiler. A handful require a full Xcode installation. You can install Xcode, the CLT, or both; Homebrew supports all three configurations. Downloading Xcode may require an Apple Developer account on older versions of Mac OS X. Sign up for free [here](https://developer.apple.com/register/index.action).
   
4. The one-liner installation method found on [brew.sh](https://brew.sh/) requires a Bourne-compatible shell (e.g. bash or zsh). Notably, fish, tcsh and csh will not work.
   
