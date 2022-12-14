## Fork of SeverSideUp/PHP for PHP8.2 and version v1.5.0

# Available Docker Images
This is a list of the docker images this repository creates:

| ⚙️ Variation | ✨ Version | 🚀 Size |
|--------------|------------|------------|
| cli          | [7.4](https://hub.docker.com/r/serversideup/php/tags?name=7.4-cli&page=1&ordering=-name), [8.0](https://hub.docker.com/r/serversideup/php/tags?name=8.0-cli&page=1&ordering=-name), [8.1](https://hub.docker.com/r/serversideup/php/tags?name=8.1-cli&page=1&ordering=-name) | [![Docker Image Size (tag)](https://img.shields.io/docker/image-size/serversideup/php/8.1-cli)](https://hub.docker.com/r/serversideup/php/tags?name=cli&page=1&ordering=-name) |
| fpm          | [7.4](https://hub.docker.com/r/serversideup/php/tags?name=7.4-fpm&page=1&ordering=-name), [8.0](https://hub.docker.com/r/serversideup/php/tags?name=8.0-fpm&page=1&ordering=-name), [8.1](https://hub.docker.com/r/serversideup/php/tags?name=8.1-fpm&page=1&ordering=-name)  | [![Docker Image Size (tag)](https://img.shields.io/docker/image-size/serversideup/php/8.1-fpm)](https://hub.docker.com/r/serversideup/php/tags?name=fpm&page=1&ordering=-name) |
| fpm-apache   | [7.4](https://hub.docker.com/r/serversideup/php/tags?name=7.4-fpm-apache&page=1&ordering=-name), [8.0](https://hub.docker.com/r/serversideup/php/tags?name=8.0-fpm-apache&page=1&ordering=-name), [8.1](https://hub.docker.com/r/serversideup/php/tags?name=8.1-fpm-apache&page=1&ordering=-name)   | [![Docker Image Size (tag)](https://img.shields.io/docker/image-size/serversideup/php/8.1-fpm-apache)](https://hub.docker.com/r/serversideup/php/tags?name=fpm-apache&page=1&ordering=-name) |
| fpm-nginx    | [7.4](https://hub.docker.com/r/serversideup/php/tags?name=7.4-fpm-nginx&page=1&ordering=-name), [8.0](https://hub.docker.com/r/serversideup/php/tags?name=8.0-fpm-nginx&page=1&ordering=-name), [8.1](https://hub.docker.com/r/serversideup/php/tags?name=8.1-fpm-nginx&page=1&ordering=-name)   |  [![Docker Image Size (tag)](https://img.shields.io/docker/image-size/serversideup/php/8.1-fpm-nginx)](https://hub.docker.com/r/serversideup/php/tags?name=fpm-nginx&page=1&ordering=-name) |

### Usage
Simply use this image name pattern in any of your projects:
```sh
serversideup/php:{{version}}-{{variation-name}}
```
For example... If I wanted to run **PHP 8.0** with **FPM + NGINX**, I would use this image:
```sh
serversideup/php:8.0-fpm-nginx
```


### Updates
✅ The image builds automatically run weekly (Tuesday at 0800 UTC) for latest security updates.

### How these images are built
All images are built off of the official Ubuntu 20.04 docker image. We first build our CLI image, then our FPM, etc. Here is what this looks like:

<img src="https://raw.githubusercontent.com/serversideup/docker-php/main/.github/dependency-diagram.png" alt="Dependency Diagram">

### Project credits & inspiration

#### [Chris Fidao](https://github.com/fideloper)
Majority of our knowledge came from Chris' course, [Shipping Docker](https://serversforhackers.com/shipping-docker). If you have yet to discover his content, you will be very satisfied with every course he has to offer. He's a great human being and excellent educator.

#### [PHPDocker.io](https://github.com/phpdocker-io/base-images)
This team has an excellent repository and millions of pulls per month. We really like how they structured their code.

#### [linuxserver.io](https://www.linuxserver.io/)
These guys are absolute aces when it comes to Docker development. They are a great resource for tons of open source Docker images.
