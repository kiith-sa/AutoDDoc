======
README
======

**AutoDDoc** is a Python script used that generates documentation for D 
language projects using D's builtin DDoc tool.

AutoDDoc is meant to be a simple, single file tool. It can only generate HTML,
and has some basic configuration options to set project properties, style of
the generated documentation and so on.

The goal is to make it as simple as possible to generate basic DDoc 
documentation for a project. With AutoDDoc, there is no need to write a custom
makefile or script just to handle documentation.


--------
Tutorial
--------

1. Copy the script to your project directory and move into that directory.
   Relative to this directory, module names must match their filenames,
   so e.g. module ``pkg.util`` would be in file ``./pkg/util.d`` .
2. Generate AutoDDoc configuation file. To do this, type
   ``./autoddoc.py -g``. This will generate file ``autoddoc.cfg`` .
3. Edit the configuation file. Set project name, version, output
   directory, and other parameters.
4. Generate the documentation by typing ``./autoddoc.py`` .


-----------
Dependecies 
-----------

AutoDDoc is written in Python and requires Python 3.2 or newer to run.
It also needs a D compiler (DMD by default) or some other tool capable 
of processing DDoc.


-------
Credits
-------

AutoDDoc was created by Ferdinand Majerech aka Kiith-Sa, kiithsacmp[AT]gmail.com 

Some of the CSS code and DDoc macros was created by 
`Digital Mars <http://www.digitalmars.com>`_, creators of the D programming language.

AutoDDoc was created using Vim on Kubuntu Linux, as a tool for the 
`D programming language <http://www.d-programming-language.org>`_.


-------
License
-------

AutoDDoc is released under the terms of the
`Boost Software License 1.0 <http://www.boost.org/LICENSE_1_0.txt>`_.
