FROM debian:bullseye-slim

RUN apt-get update && apt-get install -y ca-certificates dnscrypt-proxy

EXPOSE 53/tcp
EXPOSE 53/udp

USER nobody
ENTRYPOINT ["/usr/sbin/dnscrypt-proxy"]
CMD ["-config", "/etc/dnscrypt-proxy/dnscrypt-proxy.toml"]
