# Scala SBT 0.13

```bash
> docker build -t adlawson/sbt:0.13 -t adlawson/sbt:latest .
```

```bash
> alias sbt="docker run --rm -it \
    -v "$HOME/.ivy2":/root/.ivy2 \
    -v `pwd`:/src \
    adlawson/sbt:0.13"

> sbt sbtVersion
```
