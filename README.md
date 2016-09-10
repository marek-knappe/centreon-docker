centreon-docker
===============

This is a docker for Centreon. How to install a Centreon in 5 minutes ?


To run this just run: 

docker build -t centreon-docker .

docker run -p 80 -p 22 -i -t  centreon-docker supervisord


Default root password: centreon (please change it asap after install - u can ssh)
Default centreon admin user: admin/centreon
To check what ports u need to use make command 
# docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS                                          NAMES
512dfc6f7f0a        centreon-docker     "supervisord"       2 minutes ago       Up 2 minutes        0.0.0.0:32775->22/tcp, 0.0.0.0:32774->80/tcp   ecstatic_almeida

And you will get that ssh is on 32775 and http on 32774
