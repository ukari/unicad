# speedbar-git-respect
[![MELPA](https://melpa.org/packages/speedbar-git-respect-badge.svg)](https://melpa.org/#/speedbar-git-respect)

Particular respect git repo in speedbar

## About
This package will override the Emacs builtin `speedbar-file-lists` function and change its behaviour when the directory is a git repo.

The file list will show the following stuffs:
1. All directorys and files tracked by git
2. All directorys and files untracked by git but not matched in `.gitignore`

## Install

### with melpa
```
M-x package-install RET speedbar-git-respect RET
```

### build and install package local
`make` and extract package to directory `elpa` in emacs home directory

## Usage
``` elisp
(speedbar-git-respect-mode t)
```

## Screenshot
![](https://pbs.twimg.com/media/EJNJInXVAAAjYQ5?format=png&name=small)

## LICENSE
GPLv3

## About Unicode
The unicode filename or directory name won't display correct, unless disable the git's octal utf8 display.

To disable it, run `git config --global core.quotepath off`
