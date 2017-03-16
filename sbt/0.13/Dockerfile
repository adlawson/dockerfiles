FROM openjdk:8
MAINTAINER Andrew Lawson <https://adlawson.com>

ENV SBT_VERSION=0.13.13

RUN curl -L -o sbt-$SBT_VERSION.deb http://dl.bintray.com/sbt/debian/sbt-$SBT_VERSION.deb && \
    dpkg -i sbt-$SBT_VERSION.deb && \
    sbt sbtVersion

VOLUME /root/.ivy2
VOLUME /src
WORKDIR /src

ENTRYPOINT ["sbt"]
