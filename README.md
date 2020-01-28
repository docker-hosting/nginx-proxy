# nginx-proxy - The core of docker hosting

This is the base repository for docker-hosting. If you want to use docker-hosting, then this repository is the first thing you need.

First clone it into the directory, which you want to use for docker-hosting (e.g. `/var/www/`):

```bash
cd /var/www
git clone https://github.com/docker-hosting/nginx-proxy.git
```

Create the nginx-proxy network (with which nginx-proxy will find all other docker-compose applications that are on the same network):

```bash
docker network create nginx-proxy
```

The last thing you need to do is to start the nginx-proxy:

```bash
cd nginx-proxy # if you're not already in that folder
docker-compose up -d
```
