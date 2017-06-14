# docker-pxe - a Docker container running a continuous PXE server

# DOCKER HUB

https://registry.hub.docker.com/u/mcandre/docker-pxe/

# EXAMPLE

```
$ docker run -d -p 69:69/udp --cap-add=NET_ADMIN mcandre/docker-pxe
$ qemu-system-x86_64 -no-acpi -boot n -bootp tftp://$(docker-machine ip default)/pxelinux.0
```

# REQUIREMENTS

* [Docker](https://www.docker.com/)
* [qemu](http://wiki.qemu.org/Main_Page)

## Optional

* [make](http://www.gnu.org/software/make/)
* [Node.js](https://nodejs.org/en/) (for dockerlint)
* [editorconfig-cli](https://github.com/amyboyd/editorconfig-cli) (e.g. `go get github.com/amyboyd/editorconfig-cli`)
* [flcl](https://github.com/mcandre/flcl) (e.g. `go get github.com/mcandre/flcl/...`)
