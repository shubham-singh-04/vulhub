FROM tomcat:9-jre11-temurin

LABEL maintainer="phithon <root@leavesongs.com>"

RUN sed -i 's/securerandom.source=file:\/dev\/urandom/securerandom.source=file:\/dev\/.\/urandom/g' $JAVA_HOME/lib/security/java.security
