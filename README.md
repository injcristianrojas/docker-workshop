# Docker Workshop
Intro to Docker for security people

## Requirements

### Docker

Follow the instructions for your OS:

* [Linux](https://docs.docker.com/install/)
* [macOS](https://docs.docker.com/docker-for-mac/install/)
* [Windows](https://docs.docker.com/docker-for-windows/install/)

Then test it by running the following:

```shell
docker run hello-world
```

You should get the following:

```text
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
ca4f61b1923c: Pull complete
Digest: sha256:ca0eeb6fb05351dfc8759c20733c91def84cb8007aa89a5bf606bc8b315b9fc7
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.
...
```

### Docker Compose

Install Docker Compose following the instructions here: https://docs.docker.com/compose/install/

## Other preparation (optional)

If bandwidth is an issue, download the following images after Docker install:

```shell
docker pull ubuntu:bionic
docker pull nginx:1.14
docker pull nginx:1.14-alpine
docker pull php:7.2-fpm
docker pull php:7.2-fpm-alpine
docker pull metasploitframework/metasploit-framework:latest
docker pull wpscanteam/wpscan
```
