This repository container dupper template for mean stack repository `linnovate/mean <https://github.com/linnovate/mean>`_ .

Mean Stack 
==========

This template install mean stack dependencies and implements code-sync & cloud-9 development environment. Use below command to start container.

.. code-block:: bash

  # Install dupper if not present
  curl -sSL https://get.dupper.co | sh

  # Start mean stack container
  dupper dup --name=mean --template-from=https://github.com/athakwani/meanstack https://github.com/linnovate/mean.git
  
  # Start bidirectional code sync between container and your machine  
  dupper exec mean devenv <LOCAL_PATH_FOR_REPO>

  # or use cloud 9 browser based devlopment environment
  dupper exec mean c9

You can also host container in Digital Ocean or any other cloud provider using docker-machine and dupper:

.. code-block:: bash
  
  # Install docker-machine
  curl -L https://github.com/docker/machine/releases/download/v0.7.0/docker-machine-`uname -s`-`uname -m` > /usr/local/bin/docker-machine 
  chmod +x /usr/local/bin/docker-machine
  
  # Provision ubuntu host with your access token 
  docker-machine create --driver digitalocean --digitalocean-access-token=<your access token> \
  --digitalocean-image "ubuntu-14-04-x64" devenv-node
  eval $(docker-machine env devenv-node)

  # Install dupper if not present
  curl -sSL https://get.dupper.co | sh

  # Start mean stack container
  dupper dup --name=mean --template-from=https://github.com/athakwani/meanstack https://github.com/linnovate/mean.git
  
  # Start bidirectional code sync between container and your machine  
  dupper exec mean devenv <LOCAL_PATH_FOR_REPO>

  # or use cloud 9 browser based devlopment environment
  dupper exec mean c9

Start mean stack
================

Start mean stack using following command. This will start gulp in container and open brower on your machine.

.. code-block:: bash
  
  dupper exec mean deploy


