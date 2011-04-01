URM
===

**URM** is **Ubuntu Release Manager (urm)**. It manages Ubuntu releases
and switch between them without rebooting PC or using virtual machine.

Requirements
------------



Installation
------------

Use RubyGems to install **urm**:

    $ gem install urm


To install, initialize, and configure **urm** manually, follow these steps:

Make sure you have a bin/ directory in your home directory, and that it is included in your path:

    $ mkdir ~/bin
    $ PATH=~/bin:$PATH

Download the **urm** and ensure it is executable:

    $ curl https://github.com/JosephKu/urm/raw/master/scripts/urm > ~/bin/urm
    $ chmod a+x ~/bin/urm


Usage
-----

Install a new release of Ubuntu by specific version:

    $ urm install hardy i386

List all installed releases of Ubuntu:

    $ urm list

List all supported releases of Ubuntu:

    $ urm list --remote

Switch to a installed release of Ubuntu:

    $ urm start hardy-i386

Uninstall a installed release of Ubuntu:

    $ urm uninstall hardy-i386

Show the information of a installed release of Ubuntu:

    $ urm info hardy-i386


Contributing
------------

1. Fork it.
2. Create a branch (`git checkout -b my_urm`)
3. Commit your changes (`git commit -am "Add Ubuntu 99.04 support"`)
4. Push to the branch (`git push origin my_urm`)
5. Create an [Issue][1] with a link to your branch
6. Enjoy a refreshing Diet Coke and wait


Submitting an Issue
-------------------
I use the [GitHub issue tracker](https://github.com/JosephKu/urm/issues) to track bugs and
features. Before submitting a bug report or feature request, check to make sure it hasn't already
been submitted. You can indicate support for an existing issuse by voting it up. When submitting a
bug report, please include a [Gist](http://gist.github.com/) that includes a stack trace and any
details that may be necessary to reproduce the bug, including your gem version, Ruby version, and
operating system. Ideally, a bug report should include a pull request with failing specs.


Copyright
---------
Copyright (c) 2010-2011 Joseph Ku.
See [LICENSE](https://github.com/JosephKu/urm/blob/master/LICENSE) for details.



[1]: https://github.com/JosephKu/urm/issues

