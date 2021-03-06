# Installation

### Binary Download

Currently confd ships binaries Linux 64bit systems. You can download the latest release from [GitHub](https://github.com/joniw/confd/releases)

#### Linux

```
$ wget https://github.com/joniw/confd/releases/download/v0.12.2/confd-0.12.2-linux-amd64
```

#### Building from Source

```
$ ./build
$ sudo ./install
```

#### Building from Source for Alpine Linux

Since many people are using Alpine Linux as their base images for Docker there's support to build Alpine package also. Naturally by using Docker itself. :)

```
$ docker build -t confd_builder -f Dockerfile.build.alpine .
$ docker run -ti --rm -v $(pwd):/app confd_builder ./build
```
The above docker commands will produce binary in the local bin directory.

### Next Steps

Get up and running with the [Quick Start Guide](quick-start-guide.md).
