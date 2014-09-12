ImportWingsFile
===============

C++ Code to import Wings3D Files (See http://www.wings3d.com/)

This Project contains two classes (ErlangFile and WingsFile) which are both needed to open a wings file.
The included "main.cpp" is just an example of how to use the WingsFile class.

The wings file uses the "External Term Format" from the Erlang programming language. I haven't implemented all the datatypes of that specification. Only those that seemed to be needed by some example wings files. If you get the error "Unknown Erlang command. Maybe the file is corrupt or you are using a newer version of erts 5.7.1?", it might be that this wings file uses additional terms that aren't implemented yet. Compile this code with "-DDEBUG_WINGS" to get additional debugging information. If you want to implement this unsupported term by your own, you might also want to consider this site: "http://www.erlang.org/doc/apps/erts/erl_ext_dist.html".
