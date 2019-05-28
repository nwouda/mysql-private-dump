# mysql-private-dump
Docker image for ashleyhindle/private-dump.

See https://github.com/ashleyhindle/private-dump for the full readme for private-dump.

# using the image
Running this container will simply run private-dump, so all arguments are passed. Supplying the private-dump.json file can be done by mounting it inside the container. For example:
```
docker run --rm -v $(pwd)/private-dump.json:/private-dump.json nathanwouda/mysql-private-dump
```

To show just the help info, execute:
```
docker run --rm nathanwouda/mysql-private-dump --help
```
