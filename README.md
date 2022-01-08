
## Introduction
This is a Dockerfile to build a debian based container image running nginx and php-fpm 8.0.x / 7.4.x / 7.3.x / 7.2.x / 7.1.x / 7.0.x & Composer.

### Versioning
| Docker Tag | GitHub Release | Nginx Version | PHP Version | Debian Version | Composer
|-----|-------|-----|--------|--------|------|
| latest | master Branch |1.19.10 | 8.0.5 | buster | 2.0.13 |
| php80 | php80 Branch |1.19.10 | 8.0.5 | buster | 2.0.13 |
| php74 | php74 Branch |1.19.10 | 7.4.18 | buster | 1.10.22 |
| php73 | php73 Branch |1.19.10 | 7.3.28 | buster | 1.10.22 |
| php72 | php72 Branch |1.19.10 | 7.2.34 | buster | 1.10.22 |
| php71 | php71 Branch |1.19.10 | 7.1.33 | buster | 1.10.22 |
| php70 | php70 Branch |1.19.10 | 7.0.33 | buster | 1.10.22 |

## Building from source
To build from source you need to clone the git repo and run docker build:
```
$ git clone https://github.com/wyveo/nginx-php-fpm.git
$ cd nginx-php-fpm
```

followed by
```
$ docker build -t nginx-php-fpm:php74 . # PHP 7.4.x
```

## Pulling from Docker Hub
```
$ docker pull wyveo/nginx-php-fpm:latest
```

## Running
To run the container:
```
$ sudo docker run -d wyveo/nginx-php-fpm:latest
```

Default web root:
```
/usr/share/nginx/html
```
