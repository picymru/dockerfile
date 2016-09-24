# mongodb

A minimal, mongodb deployment based on [Alpine Linux](http://alpinelinux.org/).

## Usage

Use this as base for your own containers:

```dockerfile
FROM picymru/mongodb:latest

CMD ["/bin/sh"]
```

And install or extend with packages as you please.

## License

MIT