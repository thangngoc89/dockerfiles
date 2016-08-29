# Build

```console
docker build . --tag local-npm
```

# Run it

```console
docker run --name local-npm -d -v "$PWD/local-npm":/data -p 5080:5080 local-npm
```

# Start and add it to autostart on each start up

```console
docker start local-npm
```

# Commit it

```console
docker commit -m "Added npm" -a "Khoa Nguyen" local-npm thangngoc89/local-npm:latest
```

# Push it

```console
docker push thangngoc89/local-npm
```
