# beanstalkd-cli [![Build Status](https://travis-ci.org/EdwinHoksberg/beanstalkd-cli.svg?branch=master)](https://travis-ci.org/EdwinHoksberg/beanstalkd-cli)
A simple cli interface for managing beanstalkd queues.

## Download
You can find the latest release including binaries [here](https://github.com/bezrukov/beanstalkd-cli/releases/latest).

## Usage
```
NAME:
            beanstalkd-cli

USAGE:
            A simple cli interface for managing beanstalkd queues.

            Homepage: https://github.com/edwinhoksberg/beanstalkd-cli

VERSION:
            1.3.2 [7f1ad96f65246471eae3c07454ad8c77e6a0792f]

AUTHOR:
            Edwin Hoksberg <mail@edwinhoksberg.nl>

COMMANDS:
      monitor
            Monitor the beanstalkd queues

      flush  Completely remove all jobs from a tube

      pop    Remove a job from a queue and display it

      put    Write a job to a queue

      peek   Display a job from the queue without removing it

      help, h
            Shows a list of commands or help for one command

GLOBAL OPTIONS:
      --verbose
            set this to enable debug logging

      --quiet
            set this to disable logging

      --server value
            The server name where beanstalkd is running (default: "127.0.0.1")

      --port value
            The port on which beanstalkd is listening (default: 11300)

      --help, -h
            show help

      --version, -v
            print the version
```

## Development
This program is written in [Go](https://golang.org/), using these dependencies:
- [sirupsen/logrus](https://github.com/sirupsen/logrus) - Logrus is a structured logger for Go (golang), completely API compatible with the standard library logger.
- [urfave/cli](https://github.com/urfave/cli) - cli is a simple, fast, and fun package for building command line apps in Go.
- [mpdroog/beanstalkd](https://github.com/mpdroog/beanstalkd) - A golang beanstalkd client.

## Compile from source
This program uses Go modules which makes it easy to compile it anywhere on your system without the need for GOPATH. Just run `make build` in the project directory and it should compile without any problems.

## License
[MIT](LICENSE.md)
