# interop-docker

Repo for docker related code for modusbox images (dockerfile) and related code

Contents:

- [Deployment](#deployment)
- [Configuration](#configuration)
- [API](#api)
- [Logging](#logging)
- [Tests](#tests)

## Deployment

Steps for building:

docker build -t modusbox/mule38java8 .
flags are in the dockerfile for changing java and mule versions

For running a dev container: 

docker run -d -v /opt/mule/logs:/opt/mule/logs -p 8081:8081 -p 8088:8088 -p 9081:9081 -p 9082:9082 --name devMule -e MULE_ENV=dev modusbox/mule38java8

## Configuration

There are several configuration files:

-Dockerfile
-wrapper.conf
-ci-deploy.sh
-circle.yml

## API

This repo does not contain an API.

## Logging

Docker logs.

## Tests

There are no tests for project.
