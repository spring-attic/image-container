# Spring XD Container
This Docker image runs a Spring XD container in [distributed mode](). It expects
to connect to a ZooKeeper ensemble, an HSQLDB server and a Redis instance using
environment variables that adhere to the Docker link conventions.


Sample usage, assuming other Docker containers are running:
```
docker run --name container1 \
    --link zookeeper:zookeeper \
    --link hsqldb:hsqldb \
    --link redis:redis \
    springxd/container
```
