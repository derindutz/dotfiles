# Derin's Dotfiles

## Features
- [Install script](setup.sh)
- [OS X defaults](osx/set-defaults.sh)
- zsh aliases
- git aliases

## Installation
```sh
$ git clone https://github.com/derindutz/dotfiles.git ~/dotfiles
$ cd ~/dotfiles
$ chmod +x setup.sh
$ ./setup.sh
```

## Customize

### Local Settings

The dotfiles can be easily extended to suit additional local
requirements by using the following files:

#### `~/.zsh.local`

If the `~/.zsh.local` file exists, it will be automatically sourced
after all the other [shell related files](shell), thus, allowing its
content to add to or overwrite the existing aliases, settings, PATH,
etc.

#### `~/.gitconfig.local`

If the `~/.gitconfig.local` file exists, it will be automatically
included after the configurations from [`~/.gitconfig`](git/gitconfig), thus, allowing
its content to overwrite or add to the existing `git` configurations.

**Note:** Use `~/.gitconfig.local` to store sensitive information such
as the `git` user credentials, e.g.:

```sh
[user]
  name = Derin Dutz
  email = derin@example.com
```

## Credit

This repository is based mostly on [Nick Plekhanov's Dotfiles](https://github.com/nicksp/dotfiles)
with additions from [Mathias’s dotfiles](https://github.com/mathiasbynens/dotfiles) and other
repositories mentioned here: [GitHub ❤ ~/](http://dotfiles.github.com/).
