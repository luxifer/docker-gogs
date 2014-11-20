# Gogs in docker

## Build

```
docker build -t luxifer/gogs .
```

## Run

```
docker run -d -p 22:2222 -p 3000:3000 luxifer/gogs
```

### With data persistence

```
docker run -d -p 22:2222 -p 3000:3000 -v <somewhere>:/home/git/repositories luxifer/gogs
```
