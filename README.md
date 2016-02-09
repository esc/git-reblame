# git-reblame

Reblame ALL the commits. The bigger brother of:

https://github.com/jayphelps/git-blame-someone-else

## Install

```bash
$ git clone https://github.com/esc/git-reblame.git
$ export PATH=$PWD/git-reblame:$PATH
```

## Usage

```bash
$ git reblame <author>
```

## Disclaimer:

This changes the author and commiter of all the commits on the current branch.
The usual comments about rebase apply. Do not use in production as it will
break EVERYTHING -- Yes it's a joke command.

