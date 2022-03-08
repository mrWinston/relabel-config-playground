# Prometheus relabel config playground

This Repo helps creating and debugging prometheus relabel configs and recording
rules by running a local prometheus instance that scrapes metrics from a static
file.

## Prerequisites

* [podman](https://podman.io/) or docker
* [podman-compose](https://github.com/containers/podman-compose) or the docker equivalent

## Using this project

> This short guide will be using `podman-compose`. If you're on `docker`, you should be able to just substitute `podman-compose` with `docker-compose`.

Start the stack using podman-compose:

```
podman-compose up --force-recreate
```

This will spin up prometheus and the static metrics server. The stack looks like this:

![stack overview](./docs/overview.png)

