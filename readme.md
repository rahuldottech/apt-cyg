apt-cyg
=======

apt-cyg is a Cygwin package manager. It includes a command-line installer for
Cygwin which cooperates with Cygwin Setup and uses the same repository.

Forked from [github.com/transcode-open/apt-cyg][1]

[1]:https://github.com/transcode-open/apt-cyg

Operations
----------

~~~
install
  Install package(s).

remove
  Remove package(s) from the system.

update
  Download a fresh copy of the master package list (setup.ini) from the
  server defined in setup.rc.

download
  Retrieve package(s) from the server, but do not install/upgrade anything.

show
  Display information on given package(s).

depends
  Produce a dependency tree for a package.

rdepends
  Produce a tree of packages that depend on the named package.

list
  Search each locally-installed package for names that match regexp. If no
  package names are provided in the command line, all installed packages will
  be queried.

listall
  This will search each package in the master package list (setup.ini) for
  names that match regexp.

category
  Display all packages that are members of a named category.

listfiles
  List all files owned by a given package. Multiple packages can be specified
  on the command line.

search
  Search for downloaded packages that own the specified file(s). The path can
  be relative or absolute, and one or more files can be specified.

searchall
  Search cygwin.com to retrieve file information about packages. The provided
  target is considered to be a filename and searchall will return the
  package(s) which contain this file.
~~~

Quick start
-----------

apt-cyg is a simple script. To install:

    lynx -source https://raw.githubusercontent.com/rahuldottech/apt-cyg/master/apt-cyg > apt-cyg
    install apt-cyg /bin
    rm apt-cyg

Alternatively, if you don't have lynx installed:
    
    wget https://raw.githubusercontent.com/rahuldottech/apt-cyg/master/apt-cyg -o apt-cyg
    install apt-cyg /bin
    rm apt-cyg

Example use of apt-cyg:

    apt-cyg install nano
    

Changelog (@rahuldottech)
-----------
These are the changes which I've made to transcode-open's version:

1. Nothing till now, really, except that I updated the readme with the alternate install method and removed the rawgit link since the service is shutting down.

