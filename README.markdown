git-flow-completion
===================

Bash completion support for [git-flow](http://github.com/nvie/gitflow)

The contained completion routines provide support for completing:

 * git-flow init, feature, hotfix and release
 * feature, hotfix and release branches
 * remote feature branch names (for `git-flow feature track`)


Installation
------------

To achieve git-flow completion nirvana:

 0. Install git-completion.

 1. Install this file. Either:

    a. Place it in a `bash_completion.d` folder:

       * /etc/bash_completion.d
       * /usr/local/etc/bash_completion.d
       * ~/bash_completion.d

    b. Or, copy it somewhere (e.g. ~/.git-flow-completion.sh) and put the following line in
       your .bashrc:

           source ~/.git-flow-completion.sh

 2. If you are using Git < 1.7.1: Edit git-completion.sh and add the following line to the giant
    $command case in _git:

        flow)        _git_flow ;;


The Fine Print
--------------

Copyright (c) 2010 [Justin Hileman](http://justinhileman.com)

Distributed under the [MIT License](http://creativecommons.org/licenses/MIT/)
