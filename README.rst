pgbackup
========

Python package to manage users on a server based on an “inventory” JSON file

Preparing for Development
-------------------------

1. Ensure ``pip`` and ``pipenv`` are installed.
2. Clone repository: ``git clone https://github.com/icebreakeros/hr.git``
3. Fetch development dependencies: ``make install``

Usage
-----

The ideal usage of the hr command is this:

::
$ hr path/to/inventory.json
Adding user 'kevin'
Updating user 'lisa'
Removing user 'alex'

The alternative usage of the CLI will be to pass a --export flag like so:

::
$ hr --export path/to/inventory.json

Running Tests
-------------

Run tests locally using ``make`` if virtualenv is active:

::

    $ make

If virtualenv isn't active then use:

::

    $ pipenv run make

