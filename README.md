docker-telescope
================

[Telescope](https://github.com/TelescopeJS/Telescope) built from sources in a container based on the official [node image](https://registry.hub.docker.com/_/node/)


build it
=========

```
docker build -t telescope .
```

use it
=======

```
docker run --rm -p 3000:3000 telescope
```

making data persistent
=======================

Mount the local mongodb folder in a custom location :

```
docker run --rm -p 3000:3000 -v /some/location:/src/.meteor/local/db telescope
```
