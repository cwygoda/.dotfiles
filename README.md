# Dotfiles

## Checking out

```sh
git clone --bare <git-repo-url> $HOME/.dotfiles
git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME' checkout
```

Reload ZSH to set up `dotfiles` command alias.

## Adding files

```sh
dotfiles add .config/fancy-config-file
dotfiles commit -m "Add fancy config file"
```

## Local config files

The following files should be set up without being committed:

- `.secrets`: secret env vars like API tokens
- `.config/git/config.local`: Device specific git config, i.e. user settings
