FROM debian:bookworm-20240130-slim

RUN apt-get update && apt-get --yes install dnsmasq

COPY dnsmasq.conf /etc/

ENTRYPOINT ["dnsmasq"]

EXPOSE 53/udp
