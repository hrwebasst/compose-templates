FROM rancher/confd-base:0.11.0-dev-rancher

ADD ./conf.d /etc/confd/conf.d
ADD ./templates /etc/confd/templates
ADD ./redis.sh /usr/share/redis/rancher/redis.sh
VOLUME /usr/share/redis/rancher

ENTRYPOINT ["/confd"]

CMD ["--backend", "rancher", "--prefix", "/2015-07-25"]