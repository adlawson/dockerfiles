# Scala SBT 1.0

```bash
> docker build -t adlawson/sbt:latest -t adlawson/sbt:1.0 -t adlawson/sbt:1.0.3 .
```

```bash
> alias sbt="docker run --rm -it \
    -v "$HOME/.ivy2":/root/.ivy2 \
    -v `pwd`:/src \
    adlawson/sbt:1.0"

> sbt sbtVersion
```
