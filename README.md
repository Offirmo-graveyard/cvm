C/C++ Version Manager
=====================

XXX this project is under active development and is not yet usable XXX

C/C++ Version Manager is a tool for managing your C/C++ app with the exact components you need : compiler, libs and misc tools.

Each component is automatically installed with specific version and mode (debug/release).

C++VM is available at : https://github.com/Offirmo/cvm

Inspired from the great RVM (Ruby Version Manager) https://rvm.io//


Introduction 
============

The user story
--------------
Right now I'm writing a C++ web app. I try to deploy it to my ubuntu server. Unfortunately, it's not as simple as copying sources and compiling...

While developping, I have installed a lot of components that now need to be installed on the server as well :
- Libs. my ubuntu have packages for the libs, but of course they are outdated, so I need to download the sources and recompile last version...
- Uh oh no ! Not the last version but the same exact version my app is currently using.
- I also need the cmake tool. Of course, the default apt version is too old. So I need to download and recompile it...
- ...and so on for a lot of libs and tools...
- Oh, and I'm also planning to use latest gcc 4.7 to play with C++ 2011
- Oh, one more thing : I want to try the GNU standard lib debug mode which require recompilation of just every lib with it.

You got it. It's not only tiring to install everything again and again for each server install, it's just *impossible* at some level.

So I thought to automatize it.

I used to do some rails development, and I had a tool called "Ruby Version Manager" (RVM) which was doing exactly that for Ruby.

A quick look on the internet showed no existing tool/competitor --> Let's do this !!


Requirements
------------
C++VM is in pure shell.
C++VM need the Offirmo Shell Library  : https://github.com/Offirmo/offirmo-shell-lib

Installation
------------
Get a copy of the files and set your path to point to the "bin" dir.

Check if it works by typing : (after relaunching your shell for the PATH alteration to take effect of course !)

 `c++vm`

It should display some help.

Now you...

TODO
====

- Better doc ;)

