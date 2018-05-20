# master
Docker image hosted at: 

https://cloud.docker.com/swarm/gabriele86/repository/docker/gabriele86/devserver/general

Run image command:

docker run -i -p 22:22 -p 80:80 -p 27017:27017 -p 3306:3306 -v /Users/<cuurent_user>/Sites:/var/www/html   -t gabriele86/devserver:v1 /bin/bash -c "service apache2 start; service mysql start; service mongodb start; bash

This command create a new container with Mysql (Mapped on host port 3306 ) , Mongodb (Mapped on host port 27017 ) and Apache2  (Mapped on host port 80 ) services enabled. and create a shared value from var/www/html to /Users/<current_user>/Sites folder

"


