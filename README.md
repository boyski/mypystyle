# mypystyle
This is a convenience script to check Python code against a preferred
style (built on PEP8 and pylint).

A structural problem with both pylint and pycodestyle (a program to check
PEP8 compliance) is that they're driven by config files located in the
user's home directory. This may be convenient for the user but it means
there's no consistency of style; one user may choose to require variable
names to be at least 4 characters and another might not. A value-added
of this wrapper script is that it provides its own config files which
constitute an agreed reference standard. And since these config files are
versioned, unlike files in the home directory, changes in coding style
can be proposed, reviewed, and committed like any other coding change.

It also adds a few custom checks, like one for quote consistency,
and can check an entire directory structure if a directory is given as
an argument.

It's called "mypystyle" (vs encoding my actual name) because the style
policy is entirely in the config files; the script could easily be used
to enforce some other entity's preferred style by tweaking the configs.

I run all my Python code through this before committing and would like
contributors to my projects to do the same.

Run the script with --help for more documentation.
