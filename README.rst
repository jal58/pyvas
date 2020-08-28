pyvas: GMP for Python
=======================

|Build Status| |Coverage|

A Greenbone Managment Protocol (GMP) client for Python.

Installation
------------

To install pyvas, simply run:

.. code-block:: bash

    $ pip install pyvas

Usage
-----

.. code-block:: python

    >>> from pyvas import Client
    >>> with Client(hostname, username='username', password='password') as cli:
    >>>     r = cli.list_tasks()
    >>>     r.ok
    True
    >>>     r.data
    [{u'@id': '...', ...}, {u'@id': '...', ...}]
    >>>     r = cli.get_task(task[0]["@id"])
    >>>     r.ok
    True
    >>>     r.data
    {u'@id': '...', ...}

Documentation
-------------

Documentation is in the doc directory.


How to Contribute
-----------------

#. Look for open issues or report an issue
#. Checkout a new branch from master and work away
#. Remember to include tests
#. Submit a pull request!
