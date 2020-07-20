
### What is this ?
Quick example how to setup Keycloak, nginx and Let's Encrypt companion with docker-compose (v3).

More details in the [blog post](https://stas.starikevich.com/posts/keycloak-on-docker-with-nginx-and-letsencrypt/).

### How to start

1. Clone the repo:

```sh
  $ git clone https://github.com/kariedo/keycloak-docker-compose-example.git
```

2. adjust docker-compose.yml configuration:

- `POSTGRES_PASSWORD` should be unique and match the `DB_PASSWORD`;
- `KEYCLOAK_PASSWORD` should be unique and at least 12 characters long;
- `VIRTUAL_HOST` and `LETSENCRYPT_HOST` with the domain name from step 2;
- `LETSENCRYPT_EMAIL` with your email address;

3. spin up the containers:
```
docker-compose up
```

### Author

**Stas Starikevich**

* [github.com/kariedo](https://github.com/kariedo/)

### License

Copyright © 2020, [kariedo](https://github.com/kariedo).
