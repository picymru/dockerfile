# python3

A minimal, python3 development environment based on [Alpine Linux](http://alpinelinux.org/),
that contains pip for easy dependency management.

## Usage

Use this as base for your own containers:

```dockerfile
FROM picymru/python3:latest

CMD ["/bin/sh"]
```

And install or extend with packages as you please.

## License

MIT