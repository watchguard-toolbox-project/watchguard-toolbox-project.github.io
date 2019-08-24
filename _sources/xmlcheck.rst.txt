========
xmlcheck
========

WatchGuard policy XML check utility.

xmlcheck is used to find duplicate aliases and services 

xmlcheck is part of `WatchGuard Toolbox Project <https://watchguard-toolbox-project.github.io>`_



Installation
------------

Prerequisites
............. 

this php projects needs composer for building the class autoloader and and ensuring the SimpleXML extension is installed.

.. code-block:: shell

    ~/xmlcheck$ composer install

            Loading composer repositories with package information
            Updating dependencies (including require-dev)
            Nothing to install or update
            Writing lock file
            Generating autoload files

    ~/xmlcheck$

Usage
-----

.. code-block:: shell

    $ ./xmlcheck.php <options> <args>

Command summary
---------------

-h, --help    displays short cli help
-l, --listaliases       lists all aliases
-p, --listpolicies      lists all policies
-s, --services          lists all services
-a, --alias     print alias aliasname
--simplexmlout          print SimpleXML structure
                            as read from xmlfile

Listing aliases
---------------

.. code-block:: shell

    $ ./xmlcheck.php -i <inputxml> -l
    $ ./xmlcheck.php -i <inputxml> --listaliases

Description
...........

List all aliases from the xml file.

Options
.......

    -v, --verbose           verbose output
    -u, --unused            show only unused objects

Arguments
.........
    -i, --infile filename   inputfile filename (mandatory)


Display single alias
--------------------

.. code-block:: shell

    $ ./xmlcheck.php -i <inputxml> -a <aliasname>

Description
...........

Displays one single alias.

Options
.......

    -v, --verbose           verbose output

Arguments
.........
    -i, --infile filename   inputfile filename (mandatory)


Listing services
----------------

.. code-block:: shell

    $ ./xmlcheck.php -i <inputxml> -s
    $ ./xmlcheck.php -i <inputxml> --listservices

Description
...........

List all services from the xml file.

Options
.......

    -v, --verbose           verbose output
    -u, --unused            show only unused objects

Arguments
.........
    -i, --infile filename   inputfile filename (mandatory)


Listing policies
----------------

.. code-block:: shell

    $ ./xmlcheck.php -i <inputxml> -p
    $ ./xmlcheck.php -i <inputxml> --listpolicies

Description
...........

List all policies from the xml file.

Options
.......

    -v, --verbose           verbose output

Arguments
.........
    -i, --infile filename   inputfile filename (mandatory)


API documentation & download
----------------------------

* `phpdoc api documentation <https://watchguard-toolbox-project.github.io/xmlcheck/api/>`_
* `github repository <https://github.com/watchguard-toolbox-project/xmlcheck/>`_
