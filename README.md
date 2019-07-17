# Docker Workbench Proxy

[![](https://img.shields.io/docker/pulls/justincarter/docker-workbench-proxy.svg)](https://hub.docker.com/r/justincarter/docker-workbench-proxy 'DockerHub')

`docker-workbench-proxy` is a customised [nginx-proxy](https://hub.docker.com/r/jwilder/nginx-proxy/) container which is used as the built-in reserse proxy for [Docker Workbench](https://github.com/justincarter/docker-workbench).

Docker Workbench Proxy can be run manually in a `docker-workbench` VM using;
```
docker-machine ssh <machine-name>
docker run -d --restart=always --name=docker_workbench_proxy -p 80:80 -v '/var/run/docker.sock:/tmp/docker.sock:ro' justincarter/docker-workbench-proxy
```
