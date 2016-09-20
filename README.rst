This dupper template repository is for `Mean Stack <https://github.com/linnovate/mean>`_ + Sync development environment (devenv).

Mean stack + Sync
=================

This template install `Mean Stack <https://github.com/linnovate/mean>`_ and `Sync <https://github.com/athakwani/sync>`_. You can start mean stack with sync using below commands:

.. code-block:: bash

  dupper dup --inotify-max-watches=30000 --template-from=https://github.com/athakwani/mean-sync https://github.com/linnovate/mean
  dupper exec mean sync DIR
    
Commands
========

* start - Starts mean stack

.. code-block:: bash

    Usage:
    dupper exec mean start

* stop - Stops mean stack

.. code-block:: bash

    Usage:
    dupper exec mean stop

* logs - Display gulp output

.. code-block:: bash

    Usage:
    dupper exec mean logs

* sync - Sync mean stack code
    
.. code-block:: bash

    Usage:
    dupper exec mean sync DIR
