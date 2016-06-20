# Docker image for Docker

This image can be used to run Docker inside a Docker container, attaching to the
host Docker daemon.

Read [this](https://jpetazzo.github.io/2015/09/03/do-not-use-docker-in-docker-for-ci/)
for more information.

## Usage

```bash
$ docker run -v /var/run/docker.sock:/var/run/docker.sock \
  michelesr/docker-cli <command>
```
