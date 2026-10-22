# Container Images

PHP images based on [ServerSideUp](https://serversideup.net/open-source/docker-php/).

| Image | Tags | Upstream |
| --- | --- | --- |
| `ghcr.io/empinet/php-cli` | `8.4`, `8.5` | `serversideup/php:<version>-cli` |
| `ghcr.io/empinet/php-web` | `8.4`, `8.5` | `serversideup/php:<version>-fpm-nginx` |

Each published build also has a `<version>-build-<run-id>-<attempt>` tag.

```sh
docker run --rm ghcr.io/empinet/php-cli:8.5 php -v
```

Weekly builds skip unchanged upstream images. Pushes, pull requests, and manual runs build all images.
