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

## Example

```bash
% git clone https://github.com/jayphelps/git-blame-someone-else                                                                :(
Cloning into 'git-blame-someone-else'...
remote: Counting objects: 33, done.
remote: Compressing objects: 100% (25/25), done.
remote: Total 33 (delta 10), reused 31 (delta 8), pack-reused 0
Unpacking objects: 100% (33/33), done.
Checking connectivity... done.
% cd git-blame-someone-else 
% git --no-pager shortlog -sn 
     9  Jay Phelps
     1  Linus Torvalds
     1  Ryan Jacobs
% git reblame "Valentin Haenel <valentin@haenel.co>"
Valentin Haenel
valentin@haenel.co
Rewrite 07b4f92f3c0aacf268a40c0f489cf7392421300a (11/11)
Ref 'refs/heads/master' was rewritten
Valentin Haenel  is now the author of ALL the commits on the current branch.
Congratulations!
% git --no-pager shortlog -sn
    11  Valentin
```

## Disclaimer:

This changes the author and commiter of all the commits on the current branch.
The usual comments about rebase apply. Do not use in production as it will
break EVERYTHING -- Yes it's a joke command.

