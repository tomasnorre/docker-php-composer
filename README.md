# php-composer

PHP Containers with composer to support older PHP versions without having to install them locally. 

You can use it by running, from the directory where you want to use composer with an older PHP version. 

```bash
$ docker run --rm -ti -v $(pwd):/host-directory tomasnorre/php70-composer bash
$ cd /host-directory 
$ composer update --ignore-platform-reqs
```

The `--ignore-platform-reqs` is done as I haven't got `php70-soap` and `php70-xml` installed.
