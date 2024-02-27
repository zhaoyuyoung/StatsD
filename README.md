# StatsD [![Join the chat at https://gitter.im/statsd/statsd](https://badges.gitter.im/statsd/statsd.svg)](https://gitter.im/statsd/statsd?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Docker Pulls](https://img.shields.io/docker/pulls/statsd/statsd)](https://hub.docker.com/r/statsd/statsd)

A network daemon that runs on the [Node.js][node] platform and
listens for statistics, like counters and timers, sent over [UDP][udp] or
[TCP][tcp] and sends aggregates to one or more pluggable backend services (e.g.,
[Graphite][graphite]).

## Installation and Configuration

### Docker
StatsD supports docker in three ways:
* The official container image on [GitHub Container Registry](https://github.com/statsd/statsd/pkgs/container/statsd)
* The official container image on [DockerHub](https://hub.docker.com/r/statsd/statsd)
* Building the image from the bundled [Dockerfile](./Dockerfile)
