# lamp-docker setup

This is a simple docker compose file that configures PHP 8 + Apache. The web
server mounts volume at `{projectRoot}/public`. You can access at http://localhost:8080

It also installs the latest MySQL at localhost with no root password. It creates a
default dabase named `laravel`. MySQL mounts volume at `{projectRoot}/db` and exposes
port `3306`.

You can use phpmyadmin at http://localhost:8888.

To start the docker container:

```bash
docker/start
```

To stop the docker container:

```bash
docker/stop
```
