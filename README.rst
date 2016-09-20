This dupper template repository is for mean stack `linnovate/mean <https://github.com/linnovate/mean>`_ + Sync development environment (devenv).

Mean stack
==========

This template install `mean stack <https://github.com/linnovate/mean>`_ and `Sync devenv <https://github.com/athakwani/sync>`_. You can start mean stack devenv with below commands:

.. code-block:: bash

  dupper dup --inotify-max-watches=30000 --template-from=https://github.com/athakwani/mean-sync https://github.com/linnovate/mean
  dupper exec mean sync DIR
  
Dependencies
============

* mongodb
* nodejs
* npm
* bower
* gulp
* npm packages
* bower packages
* curl
* sudo
* inotify-tools
* openssh-server
* `gut <https://github.com/tillberg/gut>`_
    
Commands
========

* deploy - Start mean stack

.. code-block:: bash

    Usage:
    dupper exec mean deploy

* sync - Sync mean stack code
    
.. code-block:: bash

    Usage:
    dupper exec mean sync DIR
