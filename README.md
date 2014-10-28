Laptop
======

Laptop is a script to set up a Mac OS X laptop for development.

Requirements
------------

### Mac OS X

Install a C compiler:

For Lion (10.7) or Mountain Lion (10.8): use [Command Line Tools for
XCode](https://developer.apple.com/downloads/index.action).

For Mavericks (10.9): run `sudo xcodebuild -license` and follow the instructions
to accept the XCode agreement.  Then run `xcode-select --install` in your
terminal and then click "Install".

Install
-------

### Mac OS X

Read, then run the script:

    bash <(curl -s https://raw.githubusercontent.com/joshellington/laptop/master/mac)

What it sets up
---------------

* Zsh as your shell
* git for version control
* Bundler gem for managing Ruby libraries
* Heroku Config plugin for local `ENV` variables
* Heroku Toolbelt for interacting with the Heroku API
* Hub gem for interacting with the GitHub API
* Homebrew for managing operating system libraries (OS X only)
* ImageMagick for cropping and resizing images
* node.js for various dependencies
* PHP 5.5 because it's the current stable version
* Postgres for storing relational data
* MySQL for storing relational data
* Rails gem for writing web applications
* Rbenv for managing versions of the Ruby programming language
* Redis for storing key-value data
* Ruby Build for installing Rubies
* Ruby stable for writing general-purpose code
* Watch for periodically executing a program and displaying the output
* wget for easy downloading remote content
* ssh-copy-id for sending your SSH keys up to servers

It should take less than 15 minutes to install (depends on your machine).

Make your own customizations
----------------------------

Put your customizations in `~/.laptop.local`. Preferrably setup using [Homebrew Cask](http://caskroom.io/). For example, your
`~/.laptop.local` might look like this:

    #!/bin/sh

    brew tap phinze/homebrew-cask
    brew install brew-cask

    brew cask install dropbox
    brew cask install google-chrome
    brew cask install rdio

Themes
-------------

Check this resource out for iTerm2 themes: [http://iterm2colorschemes.com/](http://iterm2colorschemes.com/)

And this one for Sublimt Text themes: [http://colorsublime.com/](http://colorsublime.com/)

Dotfiles
--------

Highly recommend setting up your own dotfiles repository. Good starting point: [https://github.com/thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles)

Credits
-------

![thoughtbot](http://thoughtbot.com/assets/tm/logo.png)

Laptop is maintained and funded by [thoughtbot, inc](http://thoughtbot.com/community).
The names and logos for thoughtbot are trademarks of thoughtbot, inc.

Thank you, [contributors](https://github.com/thoughtbot/laptop/graphs/contributors)!

Contributing
------------

Please see [CONTRIBUTING.md](https://github.com/thoughtbot/laptop/blob/master/CONTRIBUTING.md).

License
-------

Laptop is © 2011-2014 thoughtbot, inc. It is free software, and may be
redistributed under the terms specified in the LICENSE file.
