# Socks5 Proxy

- [Basic SOCKS5 proxy](https://github.com/serjs/socks5-server)

This is a basic socks5 proxy written in Go by serjs. This repo simply contains the docker compose file to boot up everything quickly. This proxy does NOT support UDP.

## How to Install

- Create a new .env file (or use the one provided by removing the .example extension) with 2 variables PROXY_USER and PROXY_PASSWORD, both in plaintext
- Start up service with `docker compose up -d`
  - - Make sure the port 1080 is open in UFW and your VPS firewall config (see your cloud host provider for instructions)

## Test
- Test the proxy with `curl -x socks://username:password@<ip_address>:1080 http://ipv4.iplocation.net`
  - Should be the IP address of your proxy
