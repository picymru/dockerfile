# base

A minimal, busybox-like container based on [Alpine Linux](http://alpinelinux.org/),
that contains [apk](http://wiki.alpinelinux.org/wiki/Alpine_Linux_package_management)
package manager to ease installation of extra packages and help you build
smaller development containers.

## Usage

Use this as base for your own containers:

```dockerfile
FROM picymru-base
RUN apk-install <pakckagename>

CMD ["/bin/sh"]
```

And install or extend with packages as you please.

## License

MIT