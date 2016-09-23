# gogs

A minimal, gogs deployment based on [Alpine Linux](http://alpinelinux.org/).

## Usage

Use this as base for your own containers:

```dockerfile
FROM picymru/gogs:latest

CMD ["/bin/sh"]
```

And install or extend with packages as you please.

## License

MIT