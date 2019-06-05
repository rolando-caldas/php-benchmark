# Linux

## PHP 5

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:5.6-cli-alpine php fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:5.6-cli-alpine php bench.php
```

## PHP 7.0

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.0-cli-alpine php fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.0-cli-alpine php bench.php
```

## PHP 7.1

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.1-cli-alpine php fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.1-cli-alpine php bench.php
```

## PHP 7.2

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.2-cli-alpine php fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.2-cli-alpine php bench.php
```

## PHP 7.3

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.3-cli-alpine php fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app php:7.3-cli-alpine php bench.php
```

## PHP 8.0

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app akondas/php:8.0-cli-alpine php fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app akondas/php:8.0-cli-alpine php bench.php
```

## PHP 8.0 JIT

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app akondas/php:8.0-cli-alpine php -d "zend_extension=opcache.so" -d "opcache.enable_cli=1" -d "opcache.jit_buffer_size=500000000" -d "opcache.jit=1235" fibo.php
```

```
docker run -it -v ${PWD}:/usr/src/app -w /usr/src/app akondas/php:8.0-cli-alpine php -d "zend_extension=opcache.so" -d "opcache.enable_cli=1" -d "opcache.jit_buffer_size=500000000" -d "opcache.jit=1235" bench.php
```
