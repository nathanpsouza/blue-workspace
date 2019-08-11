# BlueCoding docker workspace for blue_shorter

## Before all

Before run any command, you must have [docker](https://docker.com) and [docker-compose](https://docs.docker.com/compose/install/) installed on your computer.

## How to setup workspace

First, clone this repository with

```
$ git clone git@github.com:nathanpsouza/blue-workspace.git
```

Move to blue-workspace directory and clone blue-shorter project:

```
$ cd blue-workspace && git clone git@github.com:nathanpsouza/blue-shorter.git
```

## Building docker image

To build project, run:

```
$ docker-compose build app
```

## Up rails server

To run project, execute on terminal:

```
$ docker-compose up app
```

After that, you can access api through address http://localhost:3000.