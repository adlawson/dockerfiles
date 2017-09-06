FROM openjdk:8
MAINTAINER Andrew Lawson <https://adlawson.com>

ENV SCALA_VERSION=2.12.3

RUN curl -L -o scala-$SCALA_VERSION.deb http://downloads.lightbend.com/scala/$SCALA_VERSION/scala-$SCALA_VERSION.deb && \
    dpkg -i scala-$SCALA_VERSION.deb && \
    rm scala-$SCALA_VERSION.deb

VOLUME /src
WORKDIR /src

ENTRYPOINT ["scala"]
