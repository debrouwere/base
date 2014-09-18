# Base

`base` temporarily adds the current directory and all of its 
subdirectories to your `$PATH`

Think of base as the recursive version of

```shell
PATH="$PATH:." <your command here>
```

Useful when you have local executables, say, a bunch of 
utilities that relate to a project, and would like a 
convenient way to play with these on the command line
without having to `source` a new environment and without
making them globally available.

Because base will add not just your current working directory 
but also *all* of its subdirectories to $PATH, you probably don't
want to use this in your home directory or something silly
like that.

## Installation

```shell
sudo wget https://raw.githubusercontent.com/stdbrouw/consecutive/master/base -O /usr/local/bin/base;
sudo chmod +x /usr/local/bin/base;
```
