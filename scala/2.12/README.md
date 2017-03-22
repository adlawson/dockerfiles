# Scala 2.12

You probably want to use `adlawson/sbt` instead, but this is for cases where I'm
working with the scala compiler directly.

```bash
> docker build -t adlawson/scala:2.12 .
```

```bash
> alias scala="docker run --rm -it \
    -v $(pwd):/src \
    --entrypoint scala \
    adlawson/scala:2.12"

> alias scalac="docker run --rm -it \
    -v $(pwd):/src \
    --entrypoint scalac \
    adlawson/scala:2.12"

> scalac Main.scala
> scala Main
```
