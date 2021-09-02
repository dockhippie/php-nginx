# php-nginx

[![Docker Build](https://github.com/dockhippie/php-nginx/workflows/docker/badge.svg)](https://github.com/dockhippie/php-nginx/actions?query=workflow%3Adocker) [![Readme Build](https://github.com/dockhippie/php-nginx/workflows/readme/badge.svg)](https://github.com/dockhippie/php-nginx/actions?query=workflow%3Areadme) [![Docker Size](https://img.shields.io/docker/image-size/webhippie/php-nginx/latest)](#) [![Docker Pulls](https://img.shields.io/docker/pulls/webhippie/php-nginx)](https://hub.docker.com/r/webhippie/php-nginx) [![GitHub Repo](https://img.shields.io/badge/github-repo-yellowgreen)](https://github.com/dockhippie/php-nginx)

These are docker images for [PHP](https://secure.php.net) on Nginx running on our [Nginx image](https://github.com/dockhippie/nginx).

## Versions

For the available versions please look at [Docker Hub](https://hub.docker.com/r/webhippie/php-nginx/tags) or [Quay](https://quay.io/repository/webhippie/php-nginx?tab=tags) or check the existing folders within the [GitHub repository](https://github.com/dockhippie/php-nginx).

## Volumes

* /srv/www
* /etc/php8/custom.d

## Ports

* 8080

## Available environment variables

```console
PHP_ALLOW_URL_FOPEN = On
PHP_ALLOW_URL_INCLUDE = Off
PHP_COMPOSER_INSTALL = true
PHP_COMPOSER_ROOT = ${NGINX_WEBROOT}
PHP_DATE_TIMEZONE = UTC
PHP_DISPLAY_ERRORS = On
PHP_DISPLAY_STARTUP_ERRORS = On
PHP_ENABLE_DL = Off
PHP_ERROR_LOG = /proc/self/fd/2
PHP_ERROR_REPORTING = E_ALL & ~E_DEPRECATED & ~E_STRICT
PHP_EXPOSE_HEADER = On
PHP_HTML_ERRORS = On
PHP_IGNORE_REPEATED_ERRORS = Off
PHP_IGNORE_REPEATED_SOURCE = Off
PHP_LISTEN_MODE = 0660
PHP_LOG_ERRORS = On
PHP_LOG_ERRORS_MAX_LEN = 1024
PHP_LOG_LEVEL = warning
PHP_MAX_CHILDREN = 75
PHP_MAX_EXECUTION_TIME = 3600
PHP_MAX_FILE_UPLOADS = 20
PHP_MAX_INPUT_TIME = 3600
PHP_MAX_REQUESTS = 500
PHP_MEMORY_LIMIT = 512M
PHP_OUTPUT_BUFFERING = 4096
PHP_PING_PATH = /ping
PHP_PING_RESPONSE = pong
PHP_POST_MAX_SIZE = 2G
PHP_PROCESS_IDLE_TIMEOUT = 10s
PHP_REPORT_MEMLEAKS = On
PHP_SKIP_CHOWN = false
PHP_SKIP_TEMPLATES = false
PHP_STATUS_LISTEN = 0.0.0.0:9001
PHP_STATUS_PATH = /status
PHP_TRACK_ERRORS = Off
PHP_UPLOAD_MAX_FILESIZE = 2G
```

## Inherited environment variables

*  [webhippie/nginx](https://github.com/dockhippie/nginx#available-environment-variables)
*  [webhippie/alpine](https://github.com/dockhippie/alpine#available-environment-variables)

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

*  [Thomas Boerger](https://github.com/tboerger)

## License

MIT

## Copyright

```console
Copyright (c) 2015 Thomas Boerger <http://www.webhippie.de>
```
