stow_reset
=========

Command to reset stow directory, especially for the case in which the package installs symbolic links.

# Usage

    stow_reset [-nh] [-d <stow dir>] [-t <target dir>] package
    
    Arguments:
          -d <stow dir>    Set stow dir to DIR (default is current dir)
          -t <target dir>  Set target to DIR (default is parent of stow dir)
          -n               Do not actually make any filesystem changes
          -h               Print Help (this message) and exit
    
# References

* [stowでmake installしたパッケージを管理](http://rcmdnk.github.io/blog/2013/08/11/computer-linux-windows-cygwin/)



[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/rcmdnk/stowreset/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

