# Caddy Cloudflare

## Prerequisites

* Cloudflare API Token

## Instructions

### Create .env file

After cloning, update `stack.env` with your variables then `mv stack.env .env` and `chmod 600 .env` to make sure it's ready for "production" use.

The only change required is to add your Cloudflare API Token.

### Update Caddyfile

This part is up to you. Add your services as needed, see my included gitea reference as a template to work from, and of course you can always [RTFM](https://caddyserver.com/docs/).

### Create network for proxy traffic

```bash
docker network create caddy
```

### Deploy

With that done you should be able to bring up Caddy with `docker compose up -d`. Use `docker logs -f caddy` to ensure certificates get signed.

## Configuration

![Under Construction](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiomutrIinAmrMZdjNekuzcHkOEiGQdZDzjTMI7LtzK23ltG_mb-YE5XDQXXxCeAAxJoXn37QUGAeKrzfIbd78N-BvB7Pn1R4D20EkQgp5uyGQR-O8Ccv833YIXiJYdGdxSO02CHjv5JT5b/s1600/under+construction.jpg)