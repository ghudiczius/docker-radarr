# Radarr

> The repository has been moved to [https://gitlab.jmk.hu/docker/media/radarr](https://gitlab.jmk.hu/docker/media/radarr).

Simple docker image for Radarr without any bloat, built on the official mono image. Radarr runs as user `radarr` with `uid` and `gid` `1000` and listens on port `7878`.

## Usage

```sh
docker run --rm registry.gitlab.jmk.hu/media/radarr:<VERSION> \
  -p 7878:7878 \
  -v path/to/config:/config \
  -v path/to/downloads:/downloads \
  -v path/to/movies:/movies
```

or

```sh
docker run --rm ghudiczius/radarr:<VERSION> \
  -p 7878:7878 \
  -v path/to/config:/config \
  -v path/to/downloads:/downloads \
  -v path/to/movies:/movies
```
