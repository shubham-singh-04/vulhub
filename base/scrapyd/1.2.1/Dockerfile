FROM python:3.12.0a5-slim

LABEL maintainer="python <root@leavesongs.com>"

RUN set -ex \
    && pip install scrapyd \
    && mkdir -p /opt/scrapyd/eggs /opt/scrapyd/dbs \
    && chown -R nobody:nogroup /opt/scrapyd

COPY scrapyd.conf /opt/scrapyd/scrapyd.conf
WORKDIR /opt/scrapyd
EXPOSE 6800

CMD ["scrapyd", "-u", "nobody", "-g", "nogroup"]
