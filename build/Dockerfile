FROM node

MAINTAINER Swoops <p.vibet@gmail.com>

RUN cd /usr/src && \
    git clone https://github.com/NDVM/NDVM.git && \
    sed -i -e 's/^\(var html5Player =\) false/\1 true/' NDVM/server/server.js && \
    sed -i -e 's/checkapp true "xdg-open/$no_browser \|\| checkapp true "xdg-open/' NDVM/start.sh

WORKDIR /usr/src/NDVM

COPY entrypoint.sh .

CMD ["/bin/bash", "./entrypoint.sh"]
