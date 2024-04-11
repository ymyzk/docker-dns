FROM debian:bullseye-slim

RUN apt-get update && apt-get install -y dnsmasq

EXPOSE 53/tcp
EXPOSE 53/udp

USER nobody
CMD ["/usr/sbin/dnsmasq", "-k"]
