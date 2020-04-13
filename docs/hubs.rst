.. _hubs:

==============================
JupyterHubs in this repository
==============================

.. _hubs/datahub:

DataHub
=======

`datahub.berkeley.edu <https://datahub.berkeley.edu>`_ is the 'main' JupyterHub
for use on UC Berkeley campus. It's the largest and most active hub. It has many
Python & R packages installed.

It runs on `Google Cloud Platform <https://cloud.google.com>`_ in the ``ucb-datahub-2018``
project. You can see :ref:`all config <structure>` for it under ``deployments/datahub``.

Classes
-------

* The big `data8 <http://data8.org/>`_ class.
* Active `connector courses <https://data.berkeley.edu/education/connectors>`_
* `Data Science Modules <https://data.berkeley.edu/education/modules>`_
* `Astro 128/256 <https://astro.berkeley.edu/course-information/3958209-astronomy-data-science-laboratory>`_

This hub is also the 'default' when folks wanna use a hub for a short period of time for
any reason without super specific requirements.

Prob140 Hub
===========

A hub specifically for `prob140 <http://prob140.org/>`_. Some of the admin users
on :ref:`hubs/datahub` are students in prob140 - this would allow them to see
the work of other prob140 students. Hence, this hub is separate until JupyterHub
gains features around restricting admin use.

It runs on `Google Cloud Platform <https://cloud.google.com>`_ in the ``ucb-datahub-2018``
project. You can see :ref:`all config <structure>` for it under ``deployments/prob140``.

Data 100
========

This hub is for `Data 100 <http://www.ds100.org/>`_ which has a unique
user and grading environment. It runs on `Google Cloud Platform <https://cloud.google.com>`_ in the ``ucb-datahub-2018`` account. You can see :ref:`all config <structure>` for it under ``deployments/data100``.

Data100 also has shared folders between staff (professors and GSIs) and students. Staff, assuming they have been added as admins in ``config/common.yaml``, can see a ``shared`` and a ``shared-readwrite`` folder. Students can only see the ``shared`` folder, which is read-only. Anything that gets put in ``shared-readwrite`` is automatically viewable in ``shared``, but as read-only files. The purpose of this is to be able to share large data files instead of having one per student. 

Data 102
========

Data 102 runs on `Google Cloud Platform <https://cloud.google.com>`_ in the ``ucb-datahub-2018`` project. You can see :ref:`all config <structure>` for it under ``deployments/data102``.

Data8X Hub
==========

A hub for the `data8x course on EdX <https://www.edx.org/professional-certificate/berkeleyx-foundations-of-data-science>`_.
This hub is open to use by anyone in the world, using `LTI Authentication <https://github.com/jupyterhub/ltiauthenticator>`_
to provide login capability from inside EdX.

It runs on `Google Cloud Platform <https://cloud.google.com>`_ in the ``data8x-scratch``
project. You can see :ref:`all config <structure>` for it under ``deployments/data8x``.