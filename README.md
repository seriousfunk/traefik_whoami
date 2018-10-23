# traefik_whoami

Simple test using https://docs.traefik.io/ example

Change Host:monitor.sendthebricks.com to your domain or remove completely to use localhost

`docker-compose up -d`

`curl -H Host:blog.sendthebricks.com http://127.0.0.1`

`docker-compose up -d --scale whoami=2`

`curl -H Host:blog.sendthebricks.com http://127.0.0.1`
Note that the IP: will round-robin between the two whoami containers
