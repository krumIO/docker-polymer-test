# Docker Polymer Test

Container for Chrome, XVFB, Polymer CLI

## Clone/Build

```
$ git clone https://github.com/krumio/docker-polymer-test.git
$ cd docker-polymer-test
$ docker build . -t krumio/docker-polymer-test:latest
```

## Run - Test your elements

```
$ cd /my-cool-app
$ docker run -it -v "$(pwd):/src/" krumio/polymer-test:latest
$ > bower install && xvfb-run --auto-servernum polymer test --simpleOutput --expanded -l chrome
```