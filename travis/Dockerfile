FROM ruby
MAINTAINER Andrew Lawson <https://adlawson.com>

RUN gem install travis

VOLUME /src
WORKDIR /src

ENTRYPOINT ["travis"]
