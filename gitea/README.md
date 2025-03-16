# Gitea

## Prerequisites

* [Caddy](https://github.com/thechainercygnus/homelab-services/tree/main/caddy-cf)
* DNS Configured

## Instructions

After cloning, update `stack.env` with your variables then `mv stack.env .env` and `chmod 600 .env` to make sure it's ready for "production" use.

The only change required to test in your own environment (that I can know) is `GITEA__server__ROOT_URL`. Replace `domain.tld` with your own.

Finally, ensure you have the required networks created:

```bash
docker network create gitea-backend
```

With that done you should be able to bring up Gitea with `docker compose up -d` and browse to the FQDN you set up `https://git.domain.tld` and set up your gitea environment.

## Configuration

![Under Construction](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiomutrIinAmrMZdjNekuzcHkOEiGQdZDzjTMI7LtzK23ltG_mb-YE5XDQXXxCeAAxJoXn37QUGAeKrzfIbd78N-BvB7Pn1R4D20EkQgp5uyGQR-O8Ccv833YIXiJYdGdxSO02CHjv5JT5b/s1600/under+construction.jpg)