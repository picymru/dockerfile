# python2

A minimal, python2 development environment based on [Alpine Linux](http://alpinelinux.org/),
that contains pip for easy dependency management.

## Usage

Use this as base for your own containers:

```dockerfile
FROM picymru/python2

CMD ["/bin/sh"]
```

And install or extend with packages as you please.

## License

MIT