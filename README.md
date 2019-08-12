# BlueCoding docker workspace for blue_shorter

## Before all

Before run any command, you must have [docker](https://docker.com) and [docker-compose](https://docs.docker.com/compose/install/) installed on your computer.

## How to setup workspace

First, clone this repository with

```
$ git clone git@github.com:nathanpsouza/blue-workspace.git
```

Move to blue-workspace directory and clone blue-shorter and blue-shorter-app projects:

```
$ cd blue-workspace && git clone git@github.com:nathanpsouza/blue-shorter.git && git clone git@github.com:nathanpsouza/blue-shorter-app.git
```

## Building docker image

To build project, run:

```
$ docker-compose build app front
```

## Install frontend app dependencies

To build project, run:

```
$ docker-compose run app bash -c "yarn install"
```

## Create database and run migrations
To create database and run migrations, execute on terminal:

```
$ docker-compose run --rm app bash -c "rails db:create db:migrate"
```

## Execute backend tests

To run rspec, execute on terminal:

```
$ docker-compose run app bash -c "rspec spec"
```

After that, you can access front end app through address http://localhost:3001.

## Run project

To run project, execute on terminal:

```
$ docker-compose up front
```

After that, you can access front end app through address http://localhost:3001.