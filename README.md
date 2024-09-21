# dokku-docker_helper

Run docker commands, like docker pull with dokku. Usually you run dokku commands through sshcommands with only capable of run dokku commands, with this you can run somethings like pull.

## Example

Imagine this, you use docker images for build and deploy, you just have all running with from-image but you need to update to a new image, but you only have dokku commands for deployment. With this, you can make dokku pull a newer image from a docker registry so after that you may run dokku ps:rebuild <app>

## Installation

```
sudo dokku plugin:install https://github.com/grizmio/dokku-docker-helper.git
```

## Commands

```
docker:pull    <image> Image to pull
```

## Usage


Dokku will run docker pull <image>
```
dokku docker:pull <image>
```

## Behind the scenes

This command just runs docker commands
