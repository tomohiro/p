p
================================================================================

Anything distribution package management wrapper


Requirements
--------------------------------------------------------------------------------

Use `/bin/sh`. Tested on OSX and Ubuntu.


Installation
--------------------------------------------------------------------------------

Download to your executable path.

    $ cd $HOME/bin
    $ curl -LO https://raw.github.com/Tomohiro/p/master/p
    $ chmod +x ./p


Usage
--------------------------------------------------------------------------------

### OSX

    $ p install tmux  # brew install tmux
    $ p update        # brew update
    $ p upgrade       # brew upgrade
    $ p search tmux   # brew search tmux


### RedHat, CentOS and Oracle Linux

    $ p install tmux  # sudo yum install tmux
    $ p update        # yum check-update
    $ p upgrade       # sudo yum update
    $ p search tmux   # yum search tmux

### Debian, Ubuntu

    $ p install tmux  # sudo apt-get install tmux
    $ p update        # sudo apt-get update
    $ p upgrade       # sudo apt-get upgrade
    $ p search tmux   # apt-cache search tmux


Commands
--------------------------------------------------------------------------------

    Usage: p COMMAND [args]

    Commands:
      update                # Retrieve new lists of packages
      outdated              # List package that have an updated version available
      installed <package>   # List all installed packages for package(or all install packages with no arguments)
      search <package>      # Search for package in all avairable packages
      info <package>        # Print info for package
      depends <package>     # List dpendencies for package
      install <package>     # Install new packages
      reinstall <package>   # ReInstall packages
      upgrade <package>     # Install newer version of outdated packages
      remove <package>      # Remove packages
      purge  <package>      # Remove packages and config files
      clean                 # Erase downloaded archive files
      autoclean             # Erase old downloaded archive files
      commands              # List 'p' all commands


---

LICENSE
--------------------------------------------------------------------------------

&copy; 2012 Tomohiro, TAIRA.
This project is licensed under the MIT license.
See LICENSE for details.
