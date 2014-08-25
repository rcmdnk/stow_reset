stow_reset
=========

Command to reset stow directory, especially for the case in which the package installs symbolic links.

# Installation

On Mac, you can install scripts by [Homebrew](https://github.com/mxcl/homebrew):

    $ brew tap rcmdnk/rcmdnkpac
    $ brew install stow_reset

If you have [brew-file](https://github.com/rcmdnk/homebrew-file), add following lines to Brewfile:

    tap 'rcmdnk/rcmdnkpac'
    brew 'stow_reset'

then, do:

    $ brew file install

Or if you write like:

    tapall 'rcmdnk/rcmdnkpac'

and do `brew file install`, you will have all useful scripts in
[rcmdnkpac](https://github.com/rcmdnk/homebrew-rcmdnkpac).

You can also use an install script on the web like:

    $ curl -fsSL https://raw.github.com/rcmdnk/stow_reset/install/install.sh| sh

This will install scripts to `/usr/bin`
and you may be asked root password.

If you want to install other directory, do like:

    $ curl -fsSL https://raw.github.com/rcmdnk/stow_reset/install/install.sh|  prefix=~/usr/local/ sh

Or, simply download scripts and set where you like.
# Usage

    stow_reset [-nh] [-d <stow dir>] [-t <target dir>] package
    
    Arguments:
          -d <stow dir>    Set stow dir to DIR (default is current dir)
          -t <target dir>  Set target to DIR (default is parent of stow dir)
          -n               Do not actually make any filesystem changes
          -h               Print Help (this message) and exit
    
# References

* [stowでmake installしたパッケージを管理](http://rcmdnk.github.io/blog/2013/08/11/computer-linux-windows-cygwin/)
