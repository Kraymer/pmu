mokapot
=======

![](https://raw.githubusercontent.com/Kraymer/public/master/mokapot/cover.png)

> **/mɔːkapōt/** :
>

1. italian stove-top coffee maker with an iconic design
2. french dirty shell script doing everything but coffee

# Description

`mokapot` brings actions on top of unix commands<sup id="a1">[1](#f1)</sup> using [`percol`](https://github.com/mooz/percol)
_interactive filtering_ concept.

I love `percol` but thought it was lacking from a practical standpoint,
forcing me to manipulate `xargs` and `awk` to pipe it with others commands.

Others options would be to use aliases and bash functions but I prefer having
a single script for maintainability.

# Usage

~~~
USAGE: mokapot [OPTIONS] git_br|git_co|git_st|pg|ps
Trigger actions on top of unix commands using percol interactive selection

MODE
    git_br      delete local branches that have been merged
    git_sh      apply action (add, stash, restore) to locally modified files
    git_co      apply action (add, stash, restore) to locally modified files
    pg          drop postgres databases
    ps          kill processes

OPTIONS
    The options are passed to the underlying binary (eg 'git' for 'moka git'
~~~

---
<i id="f1">1</i> `git`, `pg` and `psql` at time of writing
