---
title: My Environments
date: 2020-01-10 19:37:46
categories:
  - Shell
tags:
  - Bash
  - Env
  - Terminal
  - ZSH
  - Shell
cover: https://i.ibb.co/X8zQsjR/executing-bash-script-on-multiple-remote-server.jpg
---

Lots of people ask for my environment. Which tool I use, what shell and plugins do I use... In this post I'd like to introduce my environments, show off my configs and shortcuts

## Shell

As my default shell I use [**Z Shell**](https://www.zsh.org/). **ZSH** is a _Unix_ shell that can be used as an interactive login shell and as a command interpreter for shell scripting. Zsh is an extended Bourne shell with many improvements, including some features of _Bash_, _ksh_, and _tcsh_.
ZSH gives me more features than Bash does. Also as you can mention, **macOS Catalina** got zsh default and they makes you to use zsh as your default.
Additionally, I use [**ohmyzsh**](https://ohmyz.sh/) framework. Oh My Zsh is a delightful, open source, community-driven framework for managing your Zsh configuration. It comes bundled with thousands of helpful functions, helpers, plugins, themes, and a few things that make you shout...


## Packet Manager

The most essential tool for developer as I know is Packet Manager. Without packet manager, you can't manage your installed interpreters, compilers, etc. Personally, for macOS I prefer using [HomeBrew](https://brew.sh/). HomeBrew is written in Ruby.
As you know, macOS comes with built-in Ruby and Brew relies on it. You can simply install HomeBrew by typing command below in Terminal:

```shell script
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
``` 

To install packages, you need to write `brew install` then write package's name. For example, `brew install python`. This command will install latest python3 on your mac.
As an other examples, these are packages that I installed on my device:

| Package          |    Cask    |
|:----------------:|:----------:|
| cmake            |    java    |
| gdbm             | powershell |
| gettext          | 
| icu4c            | 
| libidn2          |
| libunistring     |
| mosh             |
| nmap             |
| node             |
| openssl@1.1      |
| postgresql       |
| protobuf         |
| python           |
| readline         |
| sqlite           |
| wget             |
| xz               |
| yarn             |

As you can see, you can install heavy apps as java and iterm over `brew cask` command. For example, `brew install iTerm`

