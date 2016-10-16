# docker-couchbase-community
Couchbase Community 4.1.0 + CBQ Query DP3

This is a simple image based off Ubuntu 14.04 that will install a single node of Couchbase community edition, along with the the GUI version of cbq (Couchbase Query) from the Developer Preview builds.

To use with docker-compose, the following works to set a local data store in your home directory:

docker-compose.yaml:
```
version: '2'
services:
  couchbase:
    image: codemouse/docker-couchbase-community
    volumes:
      - ~/couchbase/node1:/opt/couchbase/var
    ports:
      - 4369:4369
      - 8091:8091
      - 8092:8092
      - 8093:8093
      - 8094:8094
      - 8095:8095
      - 9100:9100
      - 9101:9101
      - 9102:9102
      - 9103:9103
      - 9104:9104
      - 9105:9105
      - 9998:9998
      - 9999:9999
      - 11207:11207
      - 11209:11209
      - 11210:11210
      - 11211:11211
      - 11214:11214
      - 11215:11215
      - 18091:18091
      - 18092:18092
      - 18093:18093
```
