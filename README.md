# shelly
shelly is a simple custom shell written in C.


A custom shell that makes use of the [readline library](http://man7.org/linux/man-pages/man3/readline.3.html), for supporting history of input commands provided and tab-completion of filenames.

I have used a few sources to understand more about the readline library
other than the man pages. I wanted to take input in a manner similar to gets
and also to support history feature of terminals. The readline library allows
me to do both of these tasks easily. Line editing is supported by default.
Also tab completion of filenames is enabled by default when using readline
to take input. Apart from these additional features, all the core features of
the shell use only standard C libraries.

http://web.mit.edu/gnu/doc/html/rlman_2.html <br>
https://eli.thegreenplace.net/2016/basics-of-using-the-readline-library/

-----------------------------------------------------------------------------

Install readline using ```sudo apt-get install libreadline8 libreadline-dev```<br>
Note : Readine version changes over time. Check the latest using ```apt-cache search readline```. Currently it is 8. <br>
Compile using ```gcc shelly.c -o shelly -lreadline```. <br>
Run using ```./shelly``` (interactive mode) or ```./shelly cmds.sh``` (batch mode)

-----------------------------------------------------------------------------

version 0.3 (2020-04-14) [ Current version ] <br>
version 0.2 (2020-04-11) <br>
version 0.1 (2020-03-11) <br>

Copyright (c) 2020 subject to the BSD 3-Clause License.
