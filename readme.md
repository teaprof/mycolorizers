# How to use

1. Create directory `~/.grc`
2. Copy all files named `conf.*` and `grc.conf` to this directory 

Now, you can run any supported command with colorized output using `grc`. For example:
```
grc valgrind a.out
```

# Note
If `~/.grc/grc.conf' exists you should merge both files (append our file to the end of existsing file).

# Note 

First, `grc` script searches for `grc.conf` in different places, including `~/.grc/grc.cong`. Files `grc.conf` contain rules
how to select appropriate scheme to colorize output. This rules consists of two-line records. The first line is regexp that should match the command passes to grc and the second line is a filename.
