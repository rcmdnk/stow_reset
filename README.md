stowReset
=========

Command to reset stow directory, especially for the case in which the package installs symbolic links.

# Usage

    stowReset [-nh] [-d <stow dir>] [-t <target dir>] package
    
    Arguments:
          -d <stow dir>    Set stow dir to DIR (default is current dir)
          -t <target dir>  Set target to DIR (default is parent of stow dir)
          -n               Do not actually make any filesystem changes
          -h               Print Help (this message) and exit
    
