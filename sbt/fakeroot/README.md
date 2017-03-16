# Scala SBT Latest with fakeroot

I use this container for building service debian packages and testing SBT build
plugins that require `fakeroot` and `dpkg`.

```bash
> docker build -t adlawson/sbt:fakeroot .
```

```
> alias sbt="docker run --rm -it \
    -v "$HOME/.ivy2":/root/.ivy2 \
    -v `pwd`:/src \
    adlawson/sbt:fakeroot"

> sbt debian:packageBin
```
