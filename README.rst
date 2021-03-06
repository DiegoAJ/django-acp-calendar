=============================
ACP-Calendar
=============================

.. image:: https://badge.fury.io/py/acp-calendar.png
    :target: https://badge.fury.io/py/acp-calendar


.. image:: https://api.travis-ci.org/luiscberrocal/django-acp-calendar.svg?branch=master
    :target: https://travis-ci.org/luiscberrocal/acp-calendar


.. image:: https://coveralls.io/repos/github/luiscberrocal/django-acp-calendar/badge.svg?branch=master
    :target: https://coveralls.io/github/luiscberrocal/django-acp-calendar?branch=master


Calendar and date management for the Panama Canal

Documentation
-------------

The full documentation is at https://acp-calendar.readthedocs.org.

Quickstart
----------

Install ACP-Calendar::

    pip install acp-calendar

Then use it in a project::

    import acp_calendar

Features
--------

To get the working days pfor the Panama Canal between january 1st to january 31st 2016.

::

     import acp_calendar

     start_date = datetime.date(2016, 1,1)
     end_date = datetime.date(2016,1,31)
     working_days = ACPHoliday.get_working_days(start_date, end_date)


Running Tests
--------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install -r requirements-test.txt
    (myenv) $ python runtests.py

Builds
---------

We are using Travis for continuos integration https://travis-ci.org/luiscberrocal/django-acp-calendar/builds

For coverage we are using coveralls https://coveralls.io/github/luiscberrocal/django-acp-calendar



Credits
---------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-pypackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
