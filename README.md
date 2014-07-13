docker-jsdav
============

Dockerfile to build a jsDAV container image.

## Quick start

- You need to mount a WebDAV data store on `/home/jsdav/app/public` because you don't want to lose everything when the container is stopped.

```console
$ mkdir -p /opt/jsDAV/public
$ docker run --name=jsdav -d -p 18000:8000 -v /opt/jsDAV/public:/home/jsdav/app/public 5t111111/jsdav
```

