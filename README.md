# path

C program to manipulate colon-separated path list environment variables.

Most importantly, it removes duplicate paths from the path variables.
It just prints out the resulting path string. which can be used to set
a new path string as in: 

    PATH=`path [args]`


```
$ ./path -h

Program to manipulate PATH-like environment variables (version 3.3).

Usage: path [-var name] [-option [path ...]] ...

Options:
 -var: use the specified environment variable instead of PATH
 -a  : add following paths after current paths if not present
 -b  : add following paths before current paths if not present
 -r  : remove following paths from current paths if present
 -ra : remove and then add following paths after current paths
 -rb : remove and then add following paths before current paths
 -ma : move following paths after other current paths if present
 -mb : move following paths before other current paths if present
 -s  : set following paths as the current path
 -dd : disable any special treatment of the DOT path
 -ci : check absolute paths in the path list to see if they are invalid
 -ri : remove absolute paths from the path list which are invalid
 -cr : check whether any paths in the path list are relative
 -rr : remove relative paths from the path list
 -tp : test whether specified paths are present in the path list
 -l  : list current paths one per line instead of in one string
 -ls : list sorted current paths one per line instead of in one string
 -af : allow files in addition to directories in paths
```

## Compilation

    make

## Author

This program was written by [David Ingalls Bell](http://members.tip.net.au/~dbell/).

The source code indicates:

/*
 * Copyright (c) 2000 David I. Bell
 * Permission is granted to use, distribute, or modify this source,
 * provided that this copyright notice remains intact.
 */
 
David Ingalls Bell made it available on his homepage and I (Christophe@pallier.org), just put it on this github repository.



