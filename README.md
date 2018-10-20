# docker-neo4j

Neo4J with consul agent 

```
docker run -d \
 -e CONSUL_JOIN="consul1 consul2" \
 -e CONSUL_DC="mydc" \
 -e CONSUL_SERVICE_NAME="neo4j" \
 mikebelozorov/neo4j
```

Base image: [neo4j](https://hub.docker.com/_/neo4j/)

Additional available envs:

- CONSUL_JOIN
- CONSUL_DC
- CONSUL_SERVICE_NAME
