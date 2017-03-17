FROM python:2.7-wheezy
MAINTAINER Andrew Lawson <https://adlawson.com>

ENV ANSIBLE_VERSION=2.0.2.0

RUN pip install ansible==$ANSIBLE_VERSION && \
    ansible --version

VOLUME /src
WORKDIR /src

ENTRYPOINT ["ansible-vault"]
