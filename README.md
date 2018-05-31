# master
Docker image hosted at: 

https://cloud.docker.com/swarm/gabriele86/repository/docker/gabriele86/devserver/general

Run image command:

docker run -i -p 22:22 -p 80:80 -p 27017:27017 -p 3306:3306 -p 9200:9200 -v /Users/gabrielebassi/Sites:/var/www/html -t gabriele86/devserver:v1 /bin/bash -c "service apache2 start; service mysql start; service mongodb start; /etc/init.d/elasticsearch;  bash"

This command create a new container with Mysql (Mapped on host port 3306 ) , Mongodb (Mapped on host port 27017 ), elasticsearch (Mapped on host port 9200 ) and Apache2  (Mapped on host port 80 ) services enabled. and create a shared value from var/www/html to /Users/<current_user>/Sites folder

"


