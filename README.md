# socks5-proxy

Basic SOCKS5 proxy

## Instructions

- Start up service with `docker compose up -d`
- Test proxy with `curl -x socks://username:password@<ip_address>:8119 http://ipv4.iplocation.net`
