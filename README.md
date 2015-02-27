centreon-docker
===============

This is a docker for Centreon. How to install a Centreon in 5 minutes ?


To run this just run:
docker build -t centreon-docker .
docker run -p 80 -p 22 -i -t  centreon-docker supervisord
