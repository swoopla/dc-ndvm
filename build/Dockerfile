FROM node

MAINTAINER Swoops <p.vibet@gmail.com>

RUN cd /usr/src && \
    git clone https://github.com/NDVM/NDVM.git && \
<<<<<<< HEAD
    sed -i -e 's/^\(var html5Player =\) false/\1 true/' NDVM/server/server.js && \
=======
>>>>>>> be24f3db0388088aed40fb698ea1bc996553519b
    sed -i -e 's/checkapp true "xdg-open/$no_browser \|\| checkapp true "xdg-open/' NDVM/start.sh

WORKDIR /usr/src/NDVM

COPY entrypoint.sh .

CMD ["/bin/bash", "./entrypoint.sh"]
