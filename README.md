# containerfiles

Building container images for various things.

## sharelatex

Based on `docker.io/sharelatex/sharelatex`, but with a larger TeX Live installation (`scheme-medium`).

```sh
VERSION=6.0.1 # sharelatex upstream version
podman build -t "ghcr.io/chrisx8/sharelatex:$VERSION" --build-arg "VERSION=$VERSION" sharelatex
```
