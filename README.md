# Virtualenv Burrito

With one command, have a working [virtualenv](http://pypi.python.org/pypi/virtualenv) +
[virtualenvwrapper](http://pypi.python.org/pypi/virtualenvwrapper)
environment.

## Install

    curl -s https://github.com/brainsik/virtualenv-burrito/raw/master/virtualenv-burrito.sh | bash

## Use

See the
[virtualenvwrapper quickstart](http://www.doughellmann.com/docs/virtualenvwrapper/install.html#quick-start)
or read the
[virtualenvwrapper command reference](http://www.doughellmann.com/docs/virtualenvwrapper/command_ref.html).

### Quickstart

To create a new virtualenv:

    mkvirtualenv newname

Once activated, pip install (_without_ using sudo) whichever Python packages
you want. They'll only be available in that virtualenv. You can make as many
virtualenvs as you want.

To switch between virtualenvs:

    workon othername

## Upgrade

To upgrade to the latest virtualenv + virtualenvwrapper packages:

    virtualenv-burrito upgrade

## Why

To get Python coders coding.

Virtualenv Burrito was inspired by
[Pycon sprinters](http://us.pycon.org/2011/sprints/) who wasted time getting
virtualenv setup so they could start hacking on code. It's sadly
complicated to quickly setup the wonderful virtualenv + virtualenvwrapper
environment. Depending on your system you may end up yak shaving with
setuptools, distribute, virtualenv, virtulenvwrapper, .bashrc, PyPI,
apt-get/MacPorts, and more.

A second feature is the ability to upgrade to newer versions of virtualenv and
virtualenvwrapper with a single command.

## Limitations

Currently, [extension
points](http://www.doughellmann.com/docs/virtualenvwrapper/plugins.html#extension-points)
(e.g., postactivate) are not supported. While this doesn't affect the project
goal of getting people coding quickly, it's a cool feature, and (more
importantly) I need it for work. :-) I'll be adding support soon and making it
available via `virtualenv-burrito upgrade`.

## Caveat emptor

This simple script is meant for people who do not have virtualenv installed.

## Credits

The real hard work is done by the creators of
[Virtualenv](http://www.virtualenv.org/) and
[Virtualenvwrapper](http://www.doughellmann.com/projects/virtualenvwrapper/).
Virtualenv is maintained by [Ian Bicking](ianbicking.org/). Virtualenvwrapper
is maintained by [Doug Hellman](http://www.doughellmann.com/).
