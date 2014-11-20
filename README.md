# Gogs in docker

See what is Gogs [here](https://github.com/gogits/gogs)

## Build

### Form source

```
docker build -t luxifer/gogs .
```

### From the [docker registry](https://registry.hub.docker.com/u/luxifer/gogs/)

```
docker pull luxifer/gogs
```

## Run

```
docker run -d -p 22:2222 -p 3000:3000 luxifer/gogs
```

If you want to disable the ssh support, just donc publish the `2222` port by removing the option `-p 22:2222`

### With data persistence

```
docker run -d -p 22:2222 -p 3000:3000 -v <somewhere>:/home/git/repositories luxifer/gogs
```

## Install

Go to `<your host>:3000` and configure pour new Gogs installation!
