FROM maven:3.9-eclipse-temurin-8

LABEL maintainer="phith0n <root@leavesongs.com>"

COPY ./ /usr/src/
WORKDIR /usr/src

RUN set -ex \
    && mvn compile jetty:help

EXPOSE 8080
CMD ["mvn", "jetty:run"]
