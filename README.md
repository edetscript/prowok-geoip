# Development environment

Add the following to the main `composer.json`

```json
"repositories": [
    {
        "type": "path",
        "version": "dev-master",
        "url": "/home/dev/usefulsomebody-geoip"
    }
],
"require": [
    "usefulsomebody/geoip": "dev-master",
]

```
Then
```sh
rm -fr vendor/usefulsomebody
php composer.phar require usefulsomebody/geoip "dev-master"
```

# Production environment

Add the following to the main `composer.json`

```json
"repositories": [
    {
        "type": "vcs",
        "url": "https://github.com/usefulsomebody/prowok-geoip"
    }
],
"require": [
    "usefulsomebody/geoip": "1.0",
]

```
Then
```sh
rm -fr vendor/usefulsomebody
php composer.phar require usefulsomebody/geoip "1.0"
```

