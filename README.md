getarg
======

A portable implemention of getopt in unistd.h.
----------------------------------------------

Got argument by `char *argopt`.

`opt_string` is a string like `ab:c`, `:` means option before it has an argument.

Use `getarg()` as condition in `while () {switch () {default: break;}}` loop, it will return every single-char option, if finished return -1. If you want get a non-optional argument,
it will return 0 and set argopt to the argument.
