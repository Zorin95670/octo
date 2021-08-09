# octo

Octo is an application to register version product of an enterprise.

It provide a website to see all deployed versions.

## Installation

Checkout your wanted release you want to install.

```
git fetch --all --tags
git checkout <tag>
```

And update submodule.

```
git submodule update --init --recursive
```

This project is a combination of an api and a web-application.

This project use docker, so all intallation information, explain how to it with docker.


### Build API

Build docker image of API.

```
docker build -t octo-spy octo-spy/
```

### Build Web-application

Build docker image of Web-application.

```
docker build -t octo-board octo-board/
```

### Run project

This project provide a docker-compose to see how all bricks works.

It need 3 docker image:

- `octo-spy`
- `octo-board`
- `postgres:13.3`

## How to use it
